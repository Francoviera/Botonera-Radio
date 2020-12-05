<template>
  <div class="container">
    <div class="row">
      <!-- Blog Entries Column -->
      <div class="col-md-8">
        <h1 class="my-4">
            Botones
        </h1>

        <!-- Blog Post -->
        <div class="col-lg-4 col-md-6 mb-4">
            <div class="card h-150">
              <div class="card-body">
                <h5>Name</h5>
                <p class="card-text">Categoria</p>
                <audio src="../assets/audios/audio1.mp3" controls="controls" type="audio/mpeg" preload="preload" width="400">
                </audio>
              </div>
              <!-- <div class="card-footer">
                <small class="text-muted">&#9733; &#9733; &#9733; &#9733; &#9734;</small>
              </div> -->
            </div>
        </div>


        <!-- Pagination -->
        <ul class="pagination justify-content-center mb-4">
          <li class="page-item">
            <a class="page-link" type="button" >&larr; Anteriores</a>
          </li>
          <li class="page-item disabled">
            <a class="page-link" type="button">Siguientes &rarr;</a>
          </li>
        </ul>

      </div>

      <!-- Sidebar Widgets Column -->
      <div class="col-md-4">

        <!-- Search Widget -->
        <div class="card my-4">
          <h5 class="card-header">Buscador</h5>
          <div class="card-body">
            <div class="input-group">
              <input type="text" class="form-control" placeholder="Ingrese Aqui...">
              <span class="input-group-append">
                <button class="btn btn-secondary" type="button">Buscar!</button>
              </span>
            </div>
          </div>
        </div>
        
        <!-- Categories Widget -->
        <div class="card my-4">
          <h5 class="card-header">Categorias</h5>
          <div class="card-body">
            <div class="row">
              <div class="col-lg-6">
                <ul class="list-unstyled mb-0">
                  <li>
                    <a href="#">Humor</a>
                  </li>
                  <li>
                    <a href="#">Chistes</a>
                  </li>
                </ul>
              </div>
              <div class="col-lg-6">
                <ul class="list-unstyled mb-0">
                    <li>
                        <a href="#">Sonido raro</a>
                    </li>
                </ul>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <!-- /.row -->

  </div>
</template>

<script>
export default {
  name: 'Buttons',
  props: {
    
  },
  mounted(){
    var audio = new Audio(require("../assets/audios/2.mp3"));
    audio.play();
    audio.pause();
  }
}
</script>