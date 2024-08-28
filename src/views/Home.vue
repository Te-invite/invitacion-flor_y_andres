<script>
import PortadaVue from '@/components/portada/PortadaVue.vue';

export default {
    name: 'Home',
    components: {
        PortadaVue
    }
}
</script>
<template>
    <div class="home_container container">
        <PortadaVue />
    </div>
</template>
<style>
.home_container {
    background: var(--color__background);
    min-height: 100vh;
    min-width: 100%;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
}
</style>