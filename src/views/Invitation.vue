<script>
import SectionPortada from '@/components/SectionPortada.vue';
import Cuadrante from '@/components/timer/Cuadrante.vue';
import CurvaRight from '@/components/icon/CurvaRight.vue';
import SectionMensaje from '@/components/SectionMensaje.vue';
import SectionAsistencia from '@/components/SectionAsistencia.vue';
import SectionLugarVue from '@/components/SectionLugar.vue.vue';
import SectionHospedaje from '@/components/SectionHospedaje.vue';
import SectionDress from '@/components/SectionDress.vue';
import SectionGift from '@/components/SectionGift.vue';
import SectionMusic from '@/components/SectionMusic.vue';
import IconBanderines from '@/components/icon/IconBanderines.vue';
import Carrousel from '@/components/Carrousel.vue';
import CurvaLeft from '@/components/icon/CurvaLeft.vue';
import CurvaWhite from '@/components/icon/CurvaWhite.vue';

export default {
    name: 'Invitation',
    components: {
        SectionPortada,
        Cuadrante,
        CurvaRight,
        SectionMensaje,
        SectionAsistencia,
        SectionLugarVue,
        SectionHospedaje,
        SectionDress,
        SectionGift,
        SectionMusic,
        IconBanderines,
        Carrousel,
        CurvaLeft,
        CurvaWhite
    }

}
</script>
<template>
    <div class="container__invitacion container">
        <div class="content_invitacion">
            <div class="box1">
                <SectionPortada />
                <CurvaRight class="curv_right" />
            </div>
            <!----------------------------------------------->
            <div class="box2">
                <Cuadrante />
            </div>
        </div>
        <!----------------------------------------------->
        <div class="box3">
            <SectionMensaje />
        </div>
        <!----------------------------------------------->
        <div class="box4">
            <SectionAsistencia />
        </div>
        <!----------------------------------------------->
        <div class="box5">
            <SectionLugarVue />
        </div>
        <!----------------------------------------------->
        <div class="box_carousel">
            <CurvaLeft class="curvaL" />
            <Carrousel />
            <CurvaWhite class="curvaW" />
        </div>
        <!----------------------------------------------->
        <div class="box6">
            <SectionHospedaje />
        </div>
        <!----------------------------------------------->
        <div class="box10">
            <IconBanderines />
        </div>
        <!----------------------------------------------->
        <div class="box7">
            <SectionDress />
        </div>
        <!----------------------------------------------->
        <div class="box8">
            <SectionGift />
        </div>
        <!----------------------------------------------->
        <div class="box9">
            <SectionMusic />
        </div>
        <!----------------------------------------------->
        <div class="container__footer">
            <div class="text_desarrolladores">
                <p class="dev1">Develop by</p>
                
                <a href="https://www.instagram.com/teinviteok/" target="_blank" rel="noopener noreferrer">
                    <p class="dev2">Teinvite.io</p>
                </a>
            </div>
        </div>
        
    </div>
</template>
<style>
.container__invitacion {
    min-width: 100%;
    min-height: 100vh;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    align-items: center;
}

.content_invitacion {
    width: 100%;
    height: auto;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
}

.box1,
.box2,
.box3,
.box4,
.box5,
.box6,
.box7,
.box8,
.box10 {
    width: 100%;
    display: flex;
    justify-content: center;

}

.box10 {
    height: 50%;
}

.box3,
.box4,
.box5,
.box6,
.box7,
.box8,
.box9,
.box_carousel {
    margin-top: 2rem
}

.box1 {
    position: relative;
}

.curvaL,
.curv_right,
.curvaW {
    position: absolute;
    z-index: 2;
}

.curv_right {
    bottom: -30px;
    right: 20px;
    width: 100%;
    height: auto;
}

.box_carousel {
    position: relative;
}

.curvaL {
    top: -35px;
    left: 0px;
    width: 100%;
    height: auto;
}

.curvaW {
    bottom: -23px;
    right: 0px;
    width: 100%;
    height: auto;
}
.text_desarrolladores {
    width: 100%;
    display: flex;
    flex-direction: row;
    justify-content: flex-end;
    align-items: center;
    font-family: Montserrat;
    margin-top: 2rem;
}
.icon{
    color:var(--color-font);
    font-size: .75rem;
    margin-left: .5rem;
    border:1px solid red;
}
.dev1 {
    color: grey;
    font-size: .5rem;
}

.dev2 {
    color: black;
    font-size: .5rem;
}
@media (min-width: 768px) and (max-width: 991px) {
    .content_invitacion {
        width: 100vw;
        padding: 0;
    }

    .box1 {
        width: 100%;
    }

    .curv_right {
        right: 0;
    }

}

@media (min-width: 1025px) {
    .content_invitacion {
        width: 100vw;
    }

    .curv_right {
        right: 0;
    }
}
</style>