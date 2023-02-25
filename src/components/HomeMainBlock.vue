<template>
    <div class="main-block">
        <div class="container">
            <Header></Header>

            <home-main-block-offer class="main-block__offer"></home-main-block-offer>

            <img class="main-block__img" src="images/offer.png" alt="Dog photo">
        </div>
    </div>
</template>


<script>
import Header from '@/components/Header.vue'
import HomeMainBlockOffer from '@/components/HomeMainBlockOffer.vue'

export default {
    components: {
        Header,
        HomeMainBlockOffer,
    },
}
</script>


<style lang="scss" scoped>
.main-block {
    background: var(--yellow-linear-gradient);

    height: 100vh;
    width: 100vw;

    &__offer {
        z-index: 2;

        // margin-top: 230px;

        position: absolute;
        top: 50%;
        transform: translateY(-50%);
    }

    &__img {
        position: absolute;

        max-width: 1060px;

        bottom: 0;
        right: 0;

        z-index: 1;
    }
}

.container {
    max-width: 1410px;
    height: 100%;

    margin: 0 auto;
}
</style>