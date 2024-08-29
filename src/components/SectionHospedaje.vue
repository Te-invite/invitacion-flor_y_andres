<script>
import IconHospedaje from './icon/IconHospedaje.vue';
export default{
    name:'SectionHospedaje',
    data(){
        return{
            title:'Hospedajes'
        }
    },
    components:{
        IconHospedaje
    }
}
</script>
<template>
    <div class="asistencia__conteiner container">
        <div class="asistencia_content">
            <IconHospedaje/>
            <h1 class="title_section_hospedaje">{{ title }}</h1>
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
.title_section_hospedaje{
    font-family: var(--family__font_primary);
    color:var(--color__font_sencondary);
    font-size: var(--font-size-32);
    font-weight: 400;
    margin-bottom: 1rem;
}
.detalle{
    font-family: var(--family__font_secondary);
    color:var(--color__font_primary);
    font-size: var(--font-size-18);
    text-align: center;
    font-weight: 200;
}
.asistencia_description{
    width:80%;
    height:100%;
}
@media (min-width: 768px) and (max-width: 991px) {
    .title_section_hospedaje{
        font-size: var(--font-size-42);
    }
}
@media (min-width: 1025px) {
    .title_section_hospedaje{
        font-size: var(--font-size-64);
    }
}
</style>