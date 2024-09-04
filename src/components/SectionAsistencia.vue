<script>
import PopupAsistencia from './PopupAsistencia.vue';
import IconParty from './icon/IconParty.vue';
import Boton from './Boton.vue';
export default{
    name:'SectionAsistencia',
    data(){
        return{
            title:'Ceremonia & Fiesta',
            popup:false
            
        }
    },
    components:{
        IconParty,
        Boton,
        PopupAsistencia
    },
    methods: {
        togglePopUp(){
            this.popup = !this.popup
        }        
    }
}
</script>
<template>
    <div id="asistencia" class="asistencia__conteiner container">
        <div class="asistencia_content">
            <IconParty/>
            <h1 class="title_section_asistencia">{{ title }}</h1>
        </div>
        <div class="asistencia_description">
            <p class="detalle_asistencia">Los esperamos el día <strong><br>2 de noviembre de 2024</strong></p>
            <p class="detalle_asistencia"><strong>Comenzamos 18:00 HS.</strong><br>Te pedimos por favor que seas puntual.</p>
        </div>
        <div class="container__button">
            <PopupAsistencia v-show="popup" @close="togglePopUp()"/>
            <Boton label="CONFIRMAR ASISTENCIA" customClass="btn-mayor" @click="togglePopUp()"/>
        </div>
         <p class="detalle_asistencia3">(Confirmar hasta el 15 de octubre)</p>
        
    </div>
</template>
<style>
.asistencia__conteiner{
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    width:100%;
    margin-bottom: 2rem;
}
.asistencia_content{
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
}
.title_section_asistencia{
    font-family: var(--family__font_primary);
    color:var(--color__font_sencondary);
    font-size: var(--font-size-32);
    font-weight: 400;
    margin-bottom: 1rem;
}
.detalle_asistencia{
    font-family: var(--family__font_secondary);
    color:var(--color__font_primary);
    font-size: var(--font-size-18);
    text-align: center;
    font-weight: 200;
}
.detalle_asistencia3{
    font-family: var(--family__font_secondary);
    color:var(--color__font_primary);
    font-size: var(--font-size-16);
    text-align: center;
    font-weight: 200;
    margin-top: .3rem;
}
.asistencia_description{
    width:80%;
    height:100%;
}
@media (min-width: 768px) and (max-width: 991px) {
    .title_section_asistencia{
        font-size: var(--font-size-42);
    }
    .detalle_asistencia{
        font-size: var(--font-size-24);
    }
    .detalle_asistencia3{
    font-size: var(--font-size-18);
    }

}
@media (min-width: 1025px) {
    .title_section_asistencia{
        font-size: var(--font-size-64);
    }
    .detalle_asistencia{
        font-size: var(--font-size-24);
    }
    .detalle_asistencia3{
        font-size: var(--font-size-16);
    }
}
</style>
