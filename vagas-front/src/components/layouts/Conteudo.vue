<template>
  <div>
    <h1> {{ titulo }} </h1>
    <button @click="atualizarComponente()">Atualizar</button>
    <button @click="conteudo = 'home'">Home</button>
    <button @click="conteudo = 'publicar-vaga'">Publicar Vaga</button>
    <!-- Renderizando dinamicamnete os componentes home e publicar vagas -->
    <!-- <home></home> -->
    <!-- <publicar-vaga></publicar-vaga> -->
    <keep-alive>
      <component :is="conteudo" />

    </keep-alive>
  </div>
</template>

<script>
import Home from '@/components/views/Home.vue'
import PublicarVaga from '@/components/views/PublicarVaga.vue';
export default {
  name: 'Conteudo',
  components: {
    Home,
    PublicarVaga
  },
  data: () => ({
    teste: 'O componente foi criado',
    titulo: 'Componente Conteúdo',
    conteudo: 'home',
  }),
  methods: {
    atualizarComponente() {
      this.titulo += '*'
    },
  },
  // beforeCreate() {
  //   console.log('Antes de criar', this.teste);
  // },
  // created() {
  //   console.log('Criado', this.teste);
  // },
  // beforeMount() {
  //   console.log('Antes de montar o template');
  // },
  // mounted() {
  //   console.log('Montado');
  // },
  // beforeUpdate() {
  //   console.log('Antes de atualizar');
  // },
  // updated() {
  //   console.log('Atualizado');
  // },
  // beforeUnmount() {
  //   console.log('Antes de desmontar');
  // },
  // unmounted() {
  //   console.log('Desmontado');
  // },
  // errorCaptured() {
  //   console.log('Erro Capturado');
  // },
  // renderTracked() {
  //   console.log('Re-renderização rastreada');
  // },
  // renderTriggered() {
  //   console.log('Re-renderização acionada');
  // },
  // activated() {
  //   console.log('Componente é ativado');
  // },
  // deactivated() {
  //   console.log('Componente é desativado');
  // }
}
</script>
  
<style module>
.teste-1 {
  background-color: red;
}

#teste-2 {
  background-color: yellow;
}
</style>

