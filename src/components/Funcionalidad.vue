<template>
    <div>
  <label for="color">Color:</label>
  <input type="text" v-model="color">
  <label for="tamanio">Tamanio:</label>
  <input type="text" v-model="tamanio">
  <label for="fondo">Fondo:</label>
  <input type="text" v-model="fondo">
  <label for="texto" style="margin-top:10px">Texto:</label>
  <input type="text" v-model="texto" :style="{color : this.color, backgroundColor: this.fondo, fontSize: this.tamanio + 'px'}">
  <p>Cantidad de palabras: {{ contarPalabras }}</p>

  <table>
  <tr>
    <th>Número de pregunta</th>
    <th>Respuesta</th>
    
  </tr>
  <tr>
    <td>1</td>
    <td>b</td>
  </tr>
  <tr>
    <td>2</td>
    <td>c</td>
  </tr>
  <tr>
    <td>3</td>
    <td>b</td>
  </tr>
  <tr>
    <td>4</td>
    <td>d</td>
  </tr>
  <tr>
    <td>5</td>
    <td>d</td>
  </tr>
</table>
 </div>

</template>

<script>

  export default  {
    name: 'src-components-funcionalidad',
    props: [],
    mounted () {

    },
    data () {
      return {
        texto:'',
        color: '',
        tamanio: '',
        fondo: '',
      }
    },
    methods: {

    },
    computed: {
      contarPalabras(){
        return this.texto.trim().split(' ').length
      }
    }
}


</script>

<style scoped lang="css">
  .src-components-funcionalidad {

  }
  table, th, td {
  border:solid black;
}
</style>
