<template>
 <div>
  <h1>Componente App</h1>
  <topo />
  <conteudo/>
 </div>
</template>

<script>
import Conteudo from './components/layouts/Conteudo.vue'
import Topo from './components/layouts/Topo.vue'

export default {
  name: 'App',
  components: {
    Conteudo,
    Topo
  }
}
</script>

<style scoped>

</style>
