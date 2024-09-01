<script>
import Boton from './Boton.vue';
export default {
    name: 'Card',
  components: {
    Boton
  },
  props: {
    nombre: {
      type: String,
      required: true
    },
    mapUrl: {
      type: String,
      required: true
    },
    embedUrl: {
      type: String,
      required: true
    }
  },
  methods: {
    openMap() {
      window.open(this.mapUrl, '_blank');
    }
  }

}
</script>
<template>
    <div class="card">
    <div class="card-body">
      <div class="image-wrapper map-container">
        <iframe class="map" 
          :src="embedUrl" 
          width="100%" height="100%" style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade">
        </iframe>
      </div>
      <h5 class="card-title">{{ nombre }}</h5>
      <Boton label="¿Cómo llegar?" customClass="btn-mayor" @click="openMap()" />
    </div>
  </div>
</template>
<style>
.card {
  width: 240px;
  height: 320px;
}

.map-container {
  height: 200px;
  width: 100%;
}

.card-body {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: space-between;
}

.card-title {
  margin-top: 1rem;
}
</style>