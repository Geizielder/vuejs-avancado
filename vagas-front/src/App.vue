<template>
 <div>
  <h1>Componente App</h1>
  <button @click="desmontarComponete()">Desmontar Componente Conteúdo</button>
  <topo />
  <conteudo v-if="visibilidade"></conteudo>
 </div>
</template>

<script>
import Conteudo from '@/components/layouts/Conteudo.vue'
import Topo from '@/components/layouts/Topo.vue'

export default {
  name: 'App',
  
  data:() => ({
    visibilidade: true
  }),
  methods: {
    desmontarComponete() {
      this.visibilidade = false
    }
  },
  components: {
    Conteudo,
    Topo
  },
}
</script>

<style scoped>

</style>
