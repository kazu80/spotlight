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
            width: 5vw;
            height: 100vh;
            background: linear-gradient(to bottom, rgba(255,255,255,1) 10%,rgba(255,255,255, .1) 100%);
        }
    }

</style>