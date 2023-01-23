<template>
  <div class="card">
    <div class="card-header bg-dark text-white"> {{ titulo }} </div>
    <div class="car-body">
      <p> {{ descricao }} </p>
    </div>
    <div class="card-footer">
      <small class="text-muted"> {{ salario }} | {{ modalidade }} | {{ tipo }} | {{ publicacao }} </small>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Vaga',
  // props: ['tituloVagaTeste', 'descricaoVaga', 'salario', 'modalidade', 'tipo', 'publicacao' ],
  props: {
    titulo: {
      type: String,
      required: true,

      //Não esta funcionando
      // vadidator:(p) => {
      //   console.log('Prop:', p, p.length)
      //   if(p.length < 6) {
      //     return false
      //   }
      //   return true
      // }
    },
    descricao: {
      type: String,
      default: 'O contratante na adicionou uma d escrição para esta vaga'
    },
    salario: {
      type: [Number, String],
      required: true
    },
    modalidade: {
      type: String,
      required: true
    },
    tipo: {
      type: String,
      required: true
    },
    publicacao: {
      type: String,
      required: true
    },
  },
}
</script>