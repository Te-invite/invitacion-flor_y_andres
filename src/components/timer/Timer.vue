<script>
import Counter from './Counter.vue';
export default {
    name: 'Timer',
    components: { Counter }
};
</script>

<template>
    <div class="section__timer">
        <div class="countdown">
            <!--Cargar fecha-->
            <counter :year="2024" :month="11" :date="2" :hour="18" :minute="0" :second="0" :millisecond="31" />
        </div>
    </div>
</template>

<style scoped>
.section__timer{
    width:100%;    
}

@media (min-width: 768px) and (max-width: 991px) {}

@media (min-width: 1025px) {
    .section__timer {
        width: 100%;
    }

    .background_count {
        width: 100%;
    }
}
</style>