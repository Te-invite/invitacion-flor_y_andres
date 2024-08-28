<script>
import foto1 from '@/assets/img/foto01.png';
import Guirnalda from './icon/Guirnalda.vue';
import CurvaRight from './icon/CurvaRight.vue';
export default {
    name: 'SectionPortada',
    components: {
        Guirnalda,
        CurvaRight
    },
    data() {
        return {
            foto1,
            title: 'Florencia & Andrés',
            subtitle: '¡NOS CASAMOS!'
        }
    }
}
</script>
<template>
    <div>
        <div class="section_portada_container">
            <div class="section_portada_img">
                <img :src="foto1" alt="">
                <div class="overlay"></div>
            </div>
            <div class="section_portada_title">
                <h1 class="title__section">{{ title }}</h1>
                <h2 class="subtitle__section">{{ subtitle }}</h2>
            </div>
            <Guirnalda class="girnalda " />
            <CurvaRight class="curv_right"/>
        </div>
        
    </div>
</template>
<style>
.section_portada_container {
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100%;
    position: relative;
}

.section_portada_img {
    position: relative;
}

img {
    display: block;
    min-width: 100%;
    height: auto;
}

.overlay {
    position: absolute;
    top: 0;
    left: 0;
    min-width: 100%;
    height: 100%;
    background-color: rgba(0, 0, 0, 0.4);
    filter: blur(10px);
}

.section_portada_title {
    position: absolute;
}

.title__section,
.subtitle__section {
    color: var(--font-light);
    line-height: 100%;
    text-align: center;
}

.title__section {
    font-family: var(--family__font_primary);
    font-size: var(--font-size-32);
}

.subtitle__section {
    font-family: var(--family__font_secondary);
    font-weight: 300;
    font-size: var(--font-size-24);
}

.girnalda {
    position: absolute;
    top: 0;
    left: 50%;
    transform: translateX(-50%);
}

.curv_right {
    position: absolute;
    bottom: -30px; 
    right: 20px;
    width: 100%; 
    height: auto; 
    z-index: 10;
}
</style>