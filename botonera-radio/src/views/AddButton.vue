<template>
  <div class="container AddButton">
    <form class="p-4">
        <div class="form-group">
          <input type="text" id="name" class="form-control" placeholder="Nombre">
        </div>
        <div class="form-group">
          <label for="exampleFormControlFile1">Elije un Audio</label>
          <input type="file" class="form-control-file" id="exampleFormControlFile1">
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
  },
  data: function(){
    return{
      cargando: true,
      buttons: [],
      buttonsFiltered: [],
      filtro: "",
    }
  },
  mounted(){
    let datosDB= JSON.parse(localStorage.getItem('buttons'));
    if(datosDB === null){
      this.molinos = [];
    }else{
      this.molinos = datosDB;
    }
    this.getEstados();
  },
  methods:{
      addButton() {
        
      },
    },
}
</script>