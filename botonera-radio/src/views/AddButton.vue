<template>
  <div class="container AddButton">
    <form class="p-4">
        <div class="form-group">
            <input type="text" id="name" class="form-control" placeholder="Nombre">
        </div>
        <div class="form-group">
            <input type="file" class="form-control">
        </div>
        <button class="btn btn-success btn-block">Agregar</button>
    </form>
  </div>
</template>
<script>
// @ is an alias to /src

export default {
  name: 'AddButton',
  components: {
  }
}
</script>