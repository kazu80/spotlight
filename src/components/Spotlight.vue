<template>
    <div class="spotlight-wrapper">
        <div class="spotlight"></div>
    </div>
</template>
<script>
    export default {
        name: 'spotlight'
    }
</script>
<style lang="scss" scoped="true">
    .spotlight-wrapper {
        padding: 0 20px;

        .spotlight {
            position: relative;
            top : -10px;
            width: 5vw;
            height: 100vh;
            background: linear-gradient(to bottom, rgba(255,255,255,1) 10%,rgba(255,255,255, .1) 100%);
            transform-origin:center top;
            transform: rotate(0deg);
            animation-name: spotlight;
            animation-duration: 1800ms;
            animation-iteration-count: infinite;
            animation-timing-function: ease-in-out;
        }

        @keyframes spotlight {
            from, to {
                transform: rotate(0deg);
            }

            35%,
            50% {
                transform: rotate(-20deg);
            }
        }
    }

</style>