<script>
import IconLocation from './icon/IconLocation.vue';
import PopupBase from './PopupBase.vue';
import Boton from './Boton.vue';
export default {
    components: { 
        PopupBase,
        IconLocation,
        Boton
    },
    data() {
        return {
        infoBtn: '¿CÓMO LLEGAR?',
        modalTitle: 'Cómo llegar a la Fiesta',
        mapUrl:'https://maps.app.goo.gl/RVNysZz6pGnucmy19'
        };
    }, 
    methods:{
        openMap(){
            window.open(this.mapUrl, '_blank');
        }   
    }
};
</script>
<template>
    <popup-base :title="modalTitle" >
        <template #icon>
            <div class="circle">
                    <IconLocation class="icon__circle"/>
            </div>
        </template>
        <div class="modal-body">
            <div class="map-container">
                <iframe class="map" src="https://www.google.com/maps/embed?pb=!1m14!1m8!1m3!1d42496.49952629916!2d-60.319885!3d-38.3587795!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x95926c3863aa9643%3A0x7f10a0f45aea89a5!2sSociedad%20Rural%20de%20Tres%20Arroyos!5e1!3m2!1ses-419!2sar!4v1725227875974!5m2!1ses-419!2sar" width="400" height="300" style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>
            </div>
        </div>
        <template #footer>
            <Boton label="ABRIR APP" customClass="btn-mayor" @click="openMap()"/>
        </template>
    </popup-base>
</template>

<style scoped>
.circle {
    width: 60px;
    height: 60px;
    border-radius: 50%;
    background: var(--color__circle);
    border: 1px solid var(--color__principal_dark);
    display: flex;
    flex-direction: column;
    align-content: center;
    justify-content: center;
    z-index: 2;
}

.icon__circle{
  width:100%;
  display:flex;
  justify-content: center;
}

::placeholder{
    color:rgb(165, 165, 165);
}

.map{
    width:260px;
    height:auto;
}
@media(max-width:320px) {   
    

    .map{
        margin-top:2rem;
        width:200px;
    }
}

@media(max-width:360px) {
    
    .circle{
        width: 45px;
        height:45px;
    }
    
    
}
@media (min-width: 768px) and (max-width: 991px){
    
    .btn-primary{
        width:60%;
    }
}
@media (min-width: 1025px) {
    
    
    .circle{
        width: 90px;
        height:90px;
    }
    .pop-up-footer{
        width:100%;
    }
    .btn-primary{
        width:50%;
    }
}

</style>