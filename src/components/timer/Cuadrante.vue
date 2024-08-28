<script>
import Timer from '@/components/timer/Timer.vue';
import contador from '@/assets/img/contador_1.png';
export default{
    name:'Cuadrante',
    components:{
        Timer
    },
    data(){
        return{
            contador
        }
    }
}
</script>
<template>
    <div class="container__cuadrante">
        <Timer/>        
    </div>
</template>
<style>
.container__cuadrante{
    margin-top:2rem;
    background-image: url('../../assets/img/contador_1.png');
    background-repeat: no-repeat;
    background-size: cover;
    width:320px;
    height: 320px;
    display: flex;
    align-items: center;
    justify-content: center;
}
</style>