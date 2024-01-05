<template>
  <div class="card">

    <CardHeader v-if="header" :header="header"/>
    <div class="card-body">
      <h5 v-if="title" class="card-title">{{ title }}</h5>
      <p v-if="parrafo" class="card-text">{{ parrafo }}</p>
      <img v-if="picture" :src="picture" alt="post img" :class="detailView ? 'full-image' : 'card-img-top'">
      <ListGroup v-if="likes"/>
      <slot></slot>
      <div class="d-grid gap-2">
        <button v-for="btn in btns" :key="btn.txt" class="btn" :class="btn.class">{{ btn.txt }}</button>
        <slot name="footer"></slot>
      </div>
    </div>
  </div>
</template>
  
<script>
import CardHeader from '@/components/CardHeader.vue';
import ListGroup from '@/components/ListGroup.vue';

export default {
  components: { CardHeader, ListGroup },
  name: 'CardCom',
  props: {
    title: String,
    parrafo: String,
    btns: Array,
    picture: String,
    header: Object,
    likes: Boolean,
    detailView: {
      type: Boolean,
      default: false
    }
  }
}
</script>
  
<style scoped>
.card {
  border: none;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1), 0 8px 16px rgba(0, 0, 0, 0.1);
}

.card-img-top {
  width: 100%;
  height: 200px; /* El tamaño que desees para todas las imágenes */
  object-fit: cover;
}

.full-image {
  width: 100%;
  height: auto;
  object-fit: contain;
  /* Agrega estilos específicos para la vista de detalles según lo necesites */
}


</style>
  