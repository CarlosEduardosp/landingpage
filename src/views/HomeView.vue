<template>
  <main>
      <div class="main-content">
        <h1 class="text1">"A jornada para o sucesso começa com um único passo.<br> Tenha coragem para dar esse passo e persistência para continuar"</h1>
        <h2 class="text2">Sou Carlos Eduardo, um programador Python Fullstack<br> com experiência em Flask, MySQL e FastAPI no back-end,<br> além de Vue.js, HTML, CSS e JavaScript no front-end.<br> Estou aqui para transformar ideias em software funcional e atraente.</h2>
        <div class="btns">
          <button class="btn">Meus Projetos</button>
          <button class="btn">me contate no <br>WhattsApp</button>
        </div>
      </div>
    </main>
</template>

<script>
export default {
  name: 'Home',
 
}
</script>

<style>
main{
  height: 93vh;
  display: flex;
  justify-content: center;
  align-items: center ;
}

.main-content{
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  gap: 20px;
}
.text1{
  font-size: 25px;
  letter-spacing: 1px;
  text-align: center;
  text-transform: uppercase;
  color: #ccacf0;
}

.text2{
  font-size: 20px;
  text-align:center;
  color: #dadee0;
}

.btns{
  display: flex;
  flex-direction: row;
  gap: 20px;
  justify-content: center;
  align-items: center;
  margin-top: 20px;
}

.btn{
  width: 20vw;
  height: 10vh;
  border-radius: 15px;
  font-size: 15px;
  background-color: transparent;
  border: 1px solid #00a2ff;
  cursor: pointer;
  color: #fff;
  transition: all 2s ease;
  text-transform: uppercase;
  transform: 2ms ease-in;
  position: relative;
  z-index: 1;
}

.btn::before{
  content: '' ;
  position: absolute;
  bottom: 0px;
  left: 0px;
  width: 0px;
  height: 60px;
  background-color: #00a2ff5b;
  transition: all 1.5s ease;
  border-radius: 15px;
  font-weight: bold;
  z-index: -1;
}

.btn:hover::before{
  width: 100%;
}

.btn:hover{
  border: none;
}
</style>