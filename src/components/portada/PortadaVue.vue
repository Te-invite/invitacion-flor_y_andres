<script>
import corazon from '@/assets/img/corazon.png';
import Boton from '../Boton.vue';

export default {
    name: 'Portada',
    components: {
        Boton
    },
    data() {
        return {
            corazon,
            title: 'Florencia & Andrés'
        }
    }
}
</script>
<template>
    <div class="portada_container container">
        <div class="portada_content container">
            <div class="conteiner__heart">
                <img :src="corazon" alt="heart">
            </div>
            <span class="conteiner__title">
                <h1 class="title__portada">{{ title }}</h1>
            </span>
        </div>
        <div class="portada_content_buttom">
            <Boton label="INGRESAR" customClass="btn-mayor" />

        </div>
        
    </div>
</template>
<style>
.portada_container{
    width: 100%;
    height: 100%;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
}
.portada_content{
    display: flex;
    justify-content: center;
    align-items: center;
    margin-bottom: 1rem;
}

.conteiner__heart {
    width: inherit;
    display: flex;
    flex-direction: column;
    justify-content: center;
    position: relative;
}

.conteiner__title {
    position: absolute;
    display: flex;
    justify-content: center;
    align-items: center;
    width: 100%;
    background: var(--color__background);
    padding: 1rem 0;

}

.title__portada {
    font-family: var(--family__font_primary);
    color: var(--color__font_primary);
    font-size: var(--font-size-28);
    line-height: 100%;
    text-align: center;
}

.portada__conteiner_button {
    width: 100%;
    display: flex;
    justify-content: center;
    align-items: center;
}
.portada_content_buttom{
    width:inherit;
    display: flex;
    justify-content: center;
    margin:2rem 0;
}

@media (min-width: 768px) and (max-width: 991px) {
    .title__portada {
        font-size: var(--font-size-32);
    }
    
}
@media (min-width: 1025px) {
    .conteiner__heart{
        width:400px;
        height:auto;
    }
}
</style>