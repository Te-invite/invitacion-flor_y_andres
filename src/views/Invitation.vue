<script>
import SectionPortada from '@/components/SectionPortada.vue';

export default{
    name:'Invitation',
    components:{
        SectionPortada
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
            <SectionPortada/>
        </div>
        
        
    </div>
</template>
<style>
.container__invitacion{
    border:1px solid rebeccapurple;
    min-width:100%;
    min-height:100vh;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    align-items: center;
}
.content_invitacion{
   width: 100%;
    display: flex;
    flex-direction: column;
    justify-content: center;
    position:relative;
}

</style>