<template>
  <div>
    <h1> {{ titulo }} </h1>
    <ul>
      <li v-for="foto of fotos" :key="foto.id">
          <img :src="foto.url" :alt="foto.descricao">
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  data () {

    return{
      titulo: 'Favorite Images',
      fotos:[
        { 
        url: 'https://picsum.photos/id/237/200/200',
        descricao: 'Cachorro'
        },
        { 
        url: 'https://picsum.photos/id/238/200/200',
        descricao: 'Prédios'
        },
      ]
    }
}

}
</script>

<style>

</style>
