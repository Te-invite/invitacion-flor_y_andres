<script>
import IconDress from './icon/IconDress.vue';
export default{
    name:'SectionDress',
    data(){
        return{
            title:'Dress Code',
            detalle:'ELEGANTE'
        }
    },
    components:{
        IconDress
    }
}
</script>
<template>
    <div id="dress" class="asistencia__conteiner container">
        <div class="asistencia_content">
            <IconDress/>
            <h1 class="title_section_dress">{{ title }}</h1>
        </div>
        <div class="asistencia_description">
            <p class="detalle_dress">{{ detalle }}</p>
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
.title_section_dress{
    font-family: var(--family__font_primary);
    color:var(--color__font_sencondary);
    font-size: var(--font-size-32);
    font-weight: 400;
    margin-bottom: 1rem;
}
.detalle_dress{
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
    .title_section_dress{
        font-size: var(--font-size-42);
    }
    .detalle_dress{
        font-size: var(--font-size-24);
    }
}
@media (min-width: 1025px) {
    .title_section_dress{
        font-size: var(--font-size-64);
    }
    .detalle_dress{
        font-size: var(--font-size-24);
    }
}
</style>