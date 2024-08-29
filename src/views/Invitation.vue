<script>
import SectionPortada from '@/components/SectionPortada.vue';
import Cuadrante from '@/components/timer/Cuadrante.vue';
import CurvaRight from '@/components/icon/CurvaRight.vue';
import SectionMensaje from '@/components/SectionMensaje.vue';
export default{
    name:'Invitation',
    components:{
        SectionPortada,
        Cuadrante,
        CurvaRight,
        SectionMensaje
    }

}
</script>
<template>
    <div class="container__invitacion container">
        <div class="content_invitacion">
            <div class="box1">
                <SectionPortada/>
                <CurvaRight class="curv_right"/>
            </div>            
            <div class="box2">
                <Cuadrante/> 
            </div>
        </div>
        <div class="box3">
            <SectionMensaje/>
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
   height:auto;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
}
.box1,
.box2, .box3{
    width: 100%;
    display: flex;
    justify-content: center;

}
.box3{
    margin-top:2rem
}
.box1{
    position: relative;
}
.curv_right {
    position: absolute;
    bottom: -30px; 
    right: 20px;
    width: 100%; 
    height: auto; 
    z-index: 10;
}
@media (min-width: 768px) and (max-width: 991px) {
  .content_invitacion{
    width:100vw;
    padding: 0;
  }
  .box1{
    width:100%;
  }
  .curv_right{
    right: 0;
  }
    
}
@media (min-width: 1025px) {
    .content_invitacion{
    width:100vw;
  }
  .curv_right{
    right: 0;
  }
}

</style>