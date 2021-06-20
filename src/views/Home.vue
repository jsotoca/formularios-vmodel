<template>
  <form>
    <input type="text" class="form-control my-2" placeholder="ingrese nombre" v-model="tarea.texto" />
    <div class="form-check form-check-inline">
      <label class="form-check-label">
        <input 
          class="form-check-input" 
          type="checkbox" 
          v-model="tarea.categorias"
          value="Javascript"
          id="check1"> 
            Javascript
      </label>
    </div>
    <div class="form-check form-check-inline">
      <label class="form-check-label">
        <input 
          class="form-check-input" 
          type="checkbox" 
          v-model="tarea.categorias"
          value="Typescript"
          id="check2"> 
            Typescript
      </label>
    </div>
    <div class="form-check form-check-inline">
      <label class="form-check-label">
        <input 
          class="form-check-input" 
          type="checkbox" 
          v-model="tarea.categorias"
          value="NodeJs"
          id="check3"> 
            NodeJs
      </label>
    </div>
    <div class="mt-2">
      <div class="form-check form-check-inline">
        <label class="form-check-label">
          <input 
            class="form-check-input" 
            type="radio"  
            id="rc1"
            v-model="tarea.estado" 
            value="urgente"> 
              Urgente
        </label>
      </div>
      <div class="form-check form-check-inline">
        <label class="form-check-label">
          <input 
            class="form-check-input" 
            type="radio"  
            id="rc2"
            v-model="tarea.estado" 
            value="relax"> 
              Relax
        </label>
      </div>
    </div>
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
        categorias: ['Typescript'],
        estado: "relax"
      }
    };
  },
};
</script>
