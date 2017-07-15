<template>
    <div class="main">
        <spotlight></spotlight>
    </div>
</template>

<script>
    import Spotlight from './components/Spotlight';

    export default {
        components: {
            Spotlight
        }
    }
</script>

<style lang="scss" scoped="true">
    .main {
        width            : 100%;
        height           : 100%;
        background-color : #000000;
    }
</style>
