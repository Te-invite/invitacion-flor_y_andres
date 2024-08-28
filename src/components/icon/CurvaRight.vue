<script>
export default {
    name: 'CurvaRight'
}
</script>
<template>
    <div>
        <svg id="curvaR"  viewBox="0 0 430 71" fill="none" xmlns="http://www.w3.org/2000/svg">
            <g clip-path="url(#clip0_66_51)">
                <mask id="mask0_66_51" style="mask-type:luminance" maskUnits="userSpaceOnUse" x="-4" y="0" width="434"
                    height="71">
                    <path d="M430 0H-4V71H430V0Z" fill="white" />
                </mask>
                <g mask="url(#mask0_66_51)">
                    <path
                        d="M128.155 72.0223H449.03L450.752 42.728C450.752 42.728 375.58 4.88238 297.909 19.004C220.237 33.1257 200.19 65.8835 128.155 55.1538V72.0223Z"
                        fill="#8CA676" />
                    <path
                        d="M450.471 68.2817L448.458 30.2211C448.458 30.2211 405.995 51.996 298.592 33.976C191.189 15.9561 43.8237 -26.8388 -16.1215 33.226V68.2817H450.471Z"
                        fill="#B1C3A2" />
                    <path
                        d="M-72.2522 72.0176H473.215L470.105 32.4712C470.105 32.4712 425.142 82.776 283.604 63.256C142.067 43.7361 5.52557 -20.0789 -71.9025 61.756C-71.9025 61.756 -72.0562 65.8597 -72.2522 72.0176Z"
                        fill="white" />
                </g>
            </g>
            <defs>
                <clipPath id="clip0_66_51">
                    <rect width="434" height="71" fill="white" transform="translate(-4)" />
                </clipPath>
            </defs>
        </svg>

    </div>
</template>
<style>
#curvaR{
    width:430px;
    height:71px;
}

@media (min-width: 768px) and (max-width: 991px) {
    #curvaR{
        width:100vw;
        height: auto;
    }
}
@media (min-width: 1025px) {
    #curvaR{
        min-width:100vw;
        height: 100%;
    }
}
</style>