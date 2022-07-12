<template>
  <div>
    <Ejercicio/>
    <br>
    <table>
      <tr>
        <th>Numero de pregunta</th>
        <th>Respuesta</th>
      </tr>
      <tr>
        <td>1</td>
        <td>B</td>
      </tr>
      <tr>
        <td>2</td>
        <td>C</td>
      </tr>
      <tr>
        <td>3</td>
        <td>B</td>
      </tr>
      <tr>
        <td>4</td>
        <td>D</td>
      </tr>
      <tr>
        <td>5</td>
        <td>D</td>
      </tr>
    </table>
  </div>
</template>

<script>
import Ejercicio from './components/Ejercicio.vue'

export default {
  name: 'App',
  components: {
    Ejercicio
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
table, th, td {
    border: 1px solid black;
    border-collapse: collapse;
}

th, td {
  padding: 5px;
}
</style>
