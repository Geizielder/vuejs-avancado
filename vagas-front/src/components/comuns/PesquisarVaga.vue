<template>
  <div class="h-1oo p-5 bg-ligth border rounded-3">

    <h2>Pesquisar vagas</h2>
    <div class="row">
      <div class="col">
        <div class="form-group">
          <label>Título da vaga</label>
          <input type="text" class="form-control"
            placeholder="Pesquise por palavras chave, por exemplo, 'PHP', 'Pleno', 'Analista' ">
          <small class="form-text text-muted">Informe palavras que estejam relacinonados com o título da vaga que
            você procura</small>
        </div>

      </div>

    </div>

  </div>
</template>

<script>
export default {
  name: 'PesquisarVaga'
}
</script>