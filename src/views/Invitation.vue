<script>
import SectionPortada from '@/components/SectionPortada.vue';
import Cuadrante from '@/components/timer/Cuadrante.vue';
export default{
    name:'Invitation',
    components:{
        SectionPortada,
        Cuadrante
    },
    data(){
        return{
            
            
        }
    }

}
</script>
<template>
    <div class="container__invitacion container">
        <div class="content_invitacion">
            <div class="box1">
                <SectionPortada/>
            </div>
            <div class="box2">
                <Cuadrante/> 
            </div>
            
            
        </div>
         
    </div>
</template>
<style>
.container__invitacion{    
    min-width:100%;
    min-height:100vh;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    align-items: center;
}
.content_invitacion{
   width: 100%;
   height:100%;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: space-between;
    position:relative;
}
@media (min-width: 768px) and (max-width: 991px) {
   
}
@media (min-width: 1025px) {
}

</style>