<template>
    <div class="offer">
        <h1 class="offer-title">Здесь ты найдёшь своего друга</h1>

        <p class="offer-subtitle">Профессиональный питомник померанских шпицев <span style="font-weight: 700;">Prayd Pom</span> исполнит вашу многолетнюю мечту!</p>
    
        <button class="offer-btn" to="/">Посмотреть щенков</button>
    </div>
</template>


<script>
export default {
    
}
</script>


<style lang="scss" scoped>
    .offer {
        max-width: 570px;

        &-title {
            margin-bottom: 42px;
        }

        &-subtitle {
            font-size: 30px;
            font-weight: 500;
            line-height: 150%;
            letter-spacing: 0.015em;

            margin-bottom: 42px;
        }

        &-btn {
            color: white;
            font-weight: 700;
            font-size: 28px;

            width: 450px;
            height: 90px;

            background: var(--pink-linear-gradient);
            box-shadow: 0px 0px 15px 2px var(--light-pink);
            border-radius: 60px;
        }
    }
</style>