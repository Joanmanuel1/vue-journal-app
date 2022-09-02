<template>
  <div class="entry-title d-flex justify-content-between p-2">
    <div>
      <span class="text-success fs-3 fw-bold">02</span>
      <span class="mx-1 fs-3">Septiembre</span>
      <span class="mx-2 fs-4 fw-light">2022, Viernes</span>
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

  <div class="d-flex flex-colum px-3 h-75">
    <textarea
      name=""
      id=""
      cols="30"
      rows="10"
      placeholder="¿Que sucedió hoy?"
    ></textarea>
  </div>

  <Fab icon="fa-save" />

  <img
    src="https://thumbs.dreamstime.com/z/monta%C3%B1as-andes-cordillera-de-los-vista-desde-la-ventana-del-avi%C3%B3n-una-un-cerca-santiago-chile-165631289.jpg"
    alt="entry-picture"
  />
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
textarea {
  font-size: 20px;
  border: none;
  height: 100%;

  &:focus {
    outline: none;
  }
}

img {
  width: 200px;
  position: fixed;
  bottom: 150px;
  right: 20px;
  box-shadow: 0px 5px 10px rgba($color: black, $alpha: 0.2);
}
</style>