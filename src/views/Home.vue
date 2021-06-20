<template>
  <form>
    <input type="text" class="form-control my-2" placeholder="ingrese nombre" v-model="tarea.texto" />
  </form>
  <p>
    {{tarea}}
  </p>
</template>

<script>
export default {
  name: "Home",
  data() {
    return {
      tarea : {
        texto: "",
        descripcion: "",
        categorias: []
      }
    };
  },
};
</script>
