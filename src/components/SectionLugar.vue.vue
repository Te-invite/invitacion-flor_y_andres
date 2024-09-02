<script>
import Boton from './Boton.vue';
import PopupLocalizacion from './PopupLocalizacion.vue';
export default{
    name:'SectionLugar',
    data(){
        return{
            title:'Lugar',
            detalle1:'La Rural - Salón grande',
            detalle2:'Entrada por Ruta 3 -Tres Arroyos',
            popup: false
        }
    },
    components:{
        Boton,
        PopupLocalizacion
    },
    methods: {
        togglePopUp(){
            this.popup = !this.popup
        }        
    }
}
</script>
<template>
    <div id="lugar" class="asistencia__conteiner container">
        <div class="asistencia_content">
            <h1 class="title_section_lugar">{{ title }}</h1>
        </div>
        <div class="asistencia_description">
            <p class="detalle_lugar">{{ detalle1 }}</p>
            <p class="detalle2_lugar">{{ detalle2 }}</p>
        </div>
        <div class="container__button">
            <PopupLocalizacion v-show="popup" @close="togglePopUp()"/>
            <Boton label="¿COMO LLEGAR?" customClass="btn-mayor" @click="togglePopUp()"/>
        </div>
        
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
.title_section_lugar{
    font-family: var(--family__font_primary);
    color:var(--color__font_sencondary);
    font-size: var(--font-size-32);
    font-weight: 400;
    margin-bottom: 1rem;
}
.detalle_lugar{
    font-family: var(--family__font_secondary);
    color:var(--color__font_primary);
    font-size: var(--font-size-18);
    text-align: center;
    font-weight: 200;
}
.detalle2_lugar{
    font-family: var(--family__font_secondary);
    color:var(--color__font_primary);
    font-size: var(--font-size-12);
    text-align: center;
    font-weight: 200;
}
.asistencia_description{
    width:80%;
    height:100%;
}
@media (min-width: 768px) and (max-width: 991px) {
    .title_section_lugar{
        font-size: var(--font-size-42);
    }
    .detalle_lugar{
        font-size: var(--font-size-24);
    }
    .detalle2_lugar{
        font-size: var(--font-size-18);
    }

}
@media (min-width: 1025px) {
    .title_section_lugar{
        font-size: var(--font-size-64);
    }
    .detalle_lugar{
        font-size: var(--font-size-28);
    }
    .detalle2_lugar{
        font-size: var(--font-size-24);
    }
}
</style>