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
    width:300px;
    height: 306px;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    margin-bottom: .5rem;
}
@media (min-width: 768px) and (max-width: 991px) {
    .container__cuadrante{
        width:420px;
        height:426px;
    }

}
@media (min-width: 1025px) {
    .container__cuadrante{
        width:520px;
        height:526px;
        margin-bottom: 1rem;
    }
}
</style>