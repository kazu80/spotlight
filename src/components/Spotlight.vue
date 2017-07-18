<template>
    <div class="spotlight-wrapper">
        <div class="spotlight"></div>
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
        display: flex;
        flex-direction: row;
        justify-content: space-between;
        position: relative;
        padding: 0 20px;

        .spotlight {
            position: relative;
            top : -30px;
            width: 5vw;
            height: 200vh;
            background: linear-gradient(to bottom, rgba(255,255,255,1) 10%,rgba(255,255,255, .1) 100%);
            transform-origin:center top;
            transform: rotate(0deg);
            animation-name: spotlight;
            animation-duration: 2000ms;
            animation-iteration-count: infinite;
            animation-timing-function: ease-in-out;
        }

        .spotlight:last-child {
            right: 0;
            animation-name: spotlight2;
        }

        @keyframes spotlight {
            from, to {
                transform: rotate(0deg);
            }

            35%,
            50% {
                transform: rotate(-45deg);
            }
        }

        @keyframes spotlight2 {
            from, to {
                transform: rotate(0deg);
            }

            35%,
            50% {
                transform: rotate(45deg);
            }
        }
    }

</style>