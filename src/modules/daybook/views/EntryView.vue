<template>
  <div class="entry-title d-flex justify-content-betwen p-2">
    <div>
      <span class="text-succes fs-3 fw-bold">15</span>
      <span class="mx-1 fs-3">Julio</span>
      <span class="mx-2 fs-4 fw-light">2021, jueves</span>
    </div>
    <div>
      <button class="btn btn-danger mx-2">
        Borrar
        <i class="fa fa-trash-alt"></i>
      </button>
      <button class="btn btn-primary">
        Subir foto
        <i class="fa fa-upload"></i>
      </button>
    </div>
  </div>
  <hr />
  <div class="d-flex flex-colum px-3 h-30">
    <textarea placeholder="¿Qué sucedió hoy?" with="100%"></textarea>
  </div>
  <fab icon="fa-save"/>
  <img src="https://www.cleverfiles.com/howto/wp-content/uploads/2018/03/minion.jpg" 
  alt="entry-picture" class="img-thumbnail">
</template>

<script>
import { defineAsyncComponent } from "vue";

export default {
  components: {
    Fab: defineAsyncComponent(() => import("../components/Fab.vue")),
  },
};
</script>

<style lang="scss" scoped>
textarea{
    width: 100%;
    height: 100%;
    font-size: 20px;
    border: none;
    margin-bottom: 2rem;
    &:focus{
        outline: none;
    }
}
img{
    width: 200px;
    position: fixed;
    bottom: 150px;
    right: 20px;
    box-shadow: 0px 5px 10px rgba($color: #000000, $alpha: 0.2);
}
</style>