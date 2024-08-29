<script>
import puntilla from '@/assets/img/puntilla.png';
import ComillaApertura from './icon/ComillaApertura.vue';
import ComillaCierre from './icon/ComillaCierre.vue';
export default {
    name: 'SectionMensaje',
    components: {
        ComillaApertura,
        ComillaCierre
    },
    data() {
        return {
            puntilla,
            mensaje1:'Hay momentos en la vida que son especiales por sí solos, compartirlos con las personas que quieres, los convierte en momentos inolvidables.',
            mensaje2:'¡Gracias por acompañarnos!'
        }
    }
}
</script>
<template>
    <div class="mensaje_container">
        <div class="msj_content_text">
            <img :src="puntilla" class="puntilla" alt="Puntilla">
            <div class="mensaje_content">
                <p class="mensaje__txt">{{ mensaje1 }}</p>
                <p class="mensaje__txt">{{ mensaje2 }}</p>
            </div>
        </div>
        <ComillaApertura class="comilla1" />
        <ComillaCierre class="comilla2" />    
    </div>
    

</template>

<style>
.mensaje_container {
    width: 350px;
    height: auto;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    position:relative;
}

.puntilla {
    width: 100%;
    height: auto;
}

.msj_content_text {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    position:relative;
    width: inherit;
    height: inherit;
}

.mensaje_content{
    width:90%;
    height: 80%;
    position: absolute;
    display: flex;
    flex-direction: column;
    justify-content: center;
}
.mensaje__txt{
    color:var(--color__font_primary);
    font-size: var(--font-size-12);
    font-family: var(--family__font_secondary);
    text-align: center;
    margin: 0;
}
.comilla1,
.comilla2{
    position: absolute;
    left: 50%;
}
.comilla1{
    margin-top: 1.3rem;
    top:0;
}
.comilla2{
    bottom:0;
    margin-bottom: 1.3rem;
}
@media (min-width: 768px) and (max-width: 991px) {
    .mensaje_container {
        width: 90%;
        height: auto;
    }
    .mensaje__txt{
        font-size: var(--font-size-24);
    }
    .mensaje_content{
        width:80%;
        height: 80%;
    }
    .comilla1{
        margin-top: 3rem;
    }
    .comilla2{
        margin-bottom: 3rem;
    }
}
@media (min-width: 1025px) {
    .mensaje_container {
        width: 90%;
        height: 40%;
    }
    .mensaje__txt{
        font-size: var(--font-size-28);
    }
    .mensaje_content{
        width:80%;
        height: 75%;
    }
    .comilla1{
        margin-top: 5rem;
    }
    .comilla2{
        margin-bottom:5rem;
    }
}
</style>