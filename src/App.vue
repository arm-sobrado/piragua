<template>
  <div id="app">
    <h1><b> Cuaderno de bitácora de la piragua </b></h1>
    <br>
    <img alt="piragua logo" src="./assets/logoPiragua.jpg">
    <main msg="Cuaderno de bitácora de la piragua"/>
  
<!--  <h1>{{ msg }}</h1> -->
    <p>
      Anotaciones de las salidas con la piragua trovatoril.
    </p>  
    <ul>
      <input id="botonSuma" type="button" value="Añadir travesía"/>
      <f> &nbsp; </f>
      <input id="botonVer" type="button" value="Ver salidas"/> 
      <f> &nbsp; </f>
      <input id="botonElimina" type="button" value="Eliminar salida"/>
    </ul>

  </div>
</template>

<script>
window.onload = function() {
  document.getElementById("botonSuma").onclick=botonSuma
  document.getElementById("botonVer").onclick=botonVer
  document.getElementById("botonElimina").onclick=botonElimina
};


function botonSuma() {
var dia;
var millas;
dia=prompt('Dia de la travesía:','');
millas=prompt('Millas de la travesía:','');
alert(dia <br>  millas)

}

function botonVer() {
alert("Chequea las travesías que has realizado");
}

function botonElimina() {
alert("Elimina una travesía");
}
/* import muestra from './components/muestra.vue'

export default {
  name: 'app',
  components: {
    muestra
  }
} */
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
