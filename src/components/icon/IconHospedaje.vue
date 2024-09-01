<script>
export default{
    name:'IconHospedaje'
}
</script>
<template>
    <div>
        <svg class="location" viewBox="0 0 51 51" fill="none" xmlns="http://www.w3.org/2000/svg">
<g filter="url(#filter0_b_84_144)">
<path d="M43.7537 21.4413C43.7537 35.6362 25.5 47.8125 25.5 47.8125C25.5 47.8125 7.24622 35.6362 7.24622 21.4413C7.24622 16.6001 9.16937 11.9571 12.5926 8.5339C16.0159 5.11066 20.6588 3.1875 25.5 3.1875C30.3412 3.1875 34.9841 5.11066 38.4073 8.5339C41.8306 11.9571 43.7537 16.6001 43.7537 21.4413Z" stroke="#8CA676" stroke-width="2" stroke-miterlimit="10"/>
<path d="M19.4225 13.3237V29.5587" stroke="#8CA676" stroke-width="2" stroke-miterlimit="10"/>
<path d="M31.5775 13.3237V29.5587" stroke="#8CA676" stroke-width="2" stroke-miterlimit="10"/>
<path d="M19.4225 21.4413H31.5775" stroke="#8CA676" stroke-width="2" stroke-miterlimit="10"/>
</g>
<defs>
<filter id="filter0_b_84_144" x="-4" y="-4" width="59" height="59" filterUnits="userSpaceOnUse" color-interpolation-filters="sRGB">
<feFlood flood-opacity="0" result="BackgroundImageFix"/>
<feGaussianBlur in="BackgroundImageFix" stdDeviation="2"/>
<feComposite in2="SourceAlpha" operator="in" result="effect1_backgroundBlur_84_144"/>
<feBlend mode="normal" in="SourceGraphic" in2="effect1_backgroundBlur_84_144" result="shape"/>
</filter>
</defs>
</svg>

    </div>
</template>
<style scoped>

.location {
    width:60px;
    height:60px;
    animation: 2.5s ease 0s infinite beat;
    transform-origin: center center;
}
@keyframes beat {

    /*Animacion del corazon*/
    0%,
    50%,
    100% {
        transform: scale(1, 1);
    }

    30%,
    80% {
        transform: scale(0.92, 0.95);
    }
}

@media (min-width: 1025px) {
    .location {
        width:60px;
        height:60px;
    }
}
</style>