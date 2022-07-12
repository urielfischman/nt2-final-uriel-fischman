<template>

  <section class="src-components-ejercicio">
    
    <label for="color"> Color: </label>
    <input name="color" type="text" v-model.trim="color">
    <label for="fondo"> Fondo: </label>
    <input name="fondo" type="text" v-model.trim="fondo">
    <label for="tamanio"> Tamaño: </label>
    <input name="tamanio" type="text" v-model.trim="tamanio">
    <hr>
    <label for="texto"> Texto: </label>
    <input name="texto" type="text" v-model.trim="texto" :style="getStyle">
    <br>
    <p v-if="texto.length">Cantidad de palabras: {{getCantidadPalabras}}</p>

  </section>

</template>

<script lang="js">

  export default  {
    name: 'src-components-ejercicio',
    props: [],
    mounted () {

    },
    data () {
      return {
        texto : "",
        color: "",
        fondo: "",
        tamanio: ""
      }
    },
    methods: {

    },
    computed: {
      getStyle(){
        return {color : this.color, "background-color" : this.fondo, "font-size" : this.tamanio}
      },
      getCantidadPalabras(){
        let cant
        if(this.texto.length){
          cant = this.texto.split(" ").length
        }else{
          cant = 0
        }
        return cant
      }
    }
}


</script>

<style scoped lang="css">
  .src-components-ejercicio {

  }

</style>
