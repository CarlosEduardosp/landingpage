<script>
import HomeViewVue from './views/HomeView.vue'

export default{
  name:'App',
  components:{
    HomeViewVue
  },
  data(){
    return{
      mensagem: ''
    }
  }
}
</script>

<template>
  <div class="html">
    <header>

      <div class="menu-content">
        <h1 class="logo">Kadu - Fullstack Solution </h1>

        <nav class="menu">
          <ul class="list-itens">
            <li><a href="#">Home</a></li>
            <li><a href="#">Sobre Mim</a></li>
            <li><a href="#">Linkedin</a></li>
            <li><a href="#">Instagram</a></li>
          </ul>
        </nav>
      </div>

    </header>

    <HomeViewVue></HomeViewVue>

  </div>
</template>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Lato:wght@300;400;700&family=Roboto:wght@400;500&display=swap');

.html{
  background-color: #1e2424;
  width: 100vw;
  height: 100vh;
  font-size: 62.5%;
  color:#fff;
  font-family: 'Lato', sans-serif;
  background: linear-gradient(#0f0125cc, #161616), url(./assets/lenguaje-programacion.jpg);
  background-position: center, center;
  background-size:cover;
  background-position-y: 0px;
  background-repeat: no-repeat;
}

header{
  width: 100%;
  height: 7vh;
  padding-top: 10px;
}

.menu-content{
  display: flex;
  justify-content:space-around;
  align-items: center;
  font-size: 1rem;
}

.logo{
  font-size: 1.5rem;
  cursor: pointer;
  color: #dadee0;
}
.logo:hover{
  color: #00a2ff;
  transition: 1.5s;
}
.menu .list-itens{
  display: flex;
  list-style-type: none;
  justify-content:center;
  align-items: center;
  cursor: pointer; 
  gap: 10px;
}

.menu .list-itens li a{
  text-decoration: none;
  color: #ffffff;
  padding: 10px 20px;
  transform: 2ms ease-in;
  position: relative;
}

.menu .list-itens li a::before{
  content: '' ;
  position: absolute;
  bottom: 0px;
  left: 0px;
  width: 0px;
  height: 1px;
  background-color: #00a2ff;
  transition: all 1.5s ease;
}
.menu .list-itens li a:hover::before{
  width: 100%; 
}
.menu .list-itens li a:hover{
  color: #00a2ff;
  transition: all 1s;
}



</style>
