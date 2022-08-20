<template>
<div class="home">
<div class="texto">
  <h1>Precisa de ajuda com os preparos do seu evento?</h1>
  <button class="contato">
    Entre em contato conosco
  </button>
</div>
</div>
</template>

<style scoped>
.home{
  display: flex;
  align-items: center;
  justify-content: center;
  width: 100%;
  height: 90vh;
}
.home::before{
  content: "";
  background-image: url('src/assets/food_background_generic.jpg');
  background-size: cover;
  position: absolute;
  top: 0px;
  right: 0px;
  bottom: 0px;
  left: 0px;
  opacity: 0.5;
}
h1 {
  position: relative;
  color: #ffffff;  
  font-size: 2rem;
  text-align: center;
}
.texto{
  display: flex;
  flex-direction: column;
  font-size: 5vh;
  align-items: center;
}
.contato{
  background-color: black;
  width: 80%;
  color: #FFF;
  border: 2px solid #F28705;
  border-radius: 0px;
  padding: 2% 15%;
  display: inline-block;
  font-family: "Lucida Console", Monaco, monospace;
  font-size: 14px;
  letter-spacing: 1px;
  cursor: pointer;
  box-shadow: inset 0 0 0 0 #F28705;
  -webkit-transition: ease-out 0.4s;
  -moz-transition: ease-out 0.4s;
  transition: ease-out 0.4s;
}
 .contato:hover {
  box-shadow: inset 52vw 0 0 0 #F28705;
}
</style>
