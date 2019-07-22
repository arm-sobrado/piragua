<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <p>
      Anotaciones de las salidas con la piragua trovatoril.
    </p>  
    <ul>
      <li><input id="botonSuma" type="button" value="Añadir travesía"/></li>
      <li><input id="botonVer" type="button" value="Ver salidas"/> </li>
      <li><input id="botonElimina" type="button" value="Eliminar salida"/> </li>
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
alert("Añade una travesía");
}

function botonVer() {
alert("Chequea las travesías que has realizado");
}

function botonElimina() {
alert("Elimina una travesía");
}

export default {
  name: 'main',
  props: {
    msg: String
  }
}
 

</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
