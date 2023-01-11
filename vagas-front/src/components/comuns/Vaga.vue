<template>
  <div class="card">
    <div class="card-header bg-dark text-white"> {{ vagas.titulo }} </div>
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
  props: ['titulo', 'descricao', 'salario', 'modalidade', 'tipo', 'publicacao' ]
}
</script>