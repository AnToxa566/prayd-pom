<template>
    <div class="main-block">
        <Header></Header>
    </div>
</template>


<script>
import Header from '@/components/Header.vue'

export default {
    components: {
        Header,
    },
}
</script>


<style lang="scss" scoped>
.main-block {
    background: var(--yellow-linear-gradient);

    height: 100vh;
    width: 100vw;
}
</style>