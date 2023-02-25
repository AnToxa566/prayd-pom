<template>
    <div class="header d-flex justify-space-between align-center">
        <div class="header-logo d-flex align-center">
            <img class="header-logo__img" src="icons/logo.svg" alt="Logo">

            <h3 class="header-logo__text">Prayd Pom</h3>
        </div>

        <div class="header-menu">
            <router-link
                v-for="(link, index) in this.menuLinks"

                :key="index"
                :to="link.path"

                class="header-menu__link"
                :class="{ 'header-menu__link-active' : link.active }"
            >
                {{ link.title }}
            </router-link>
        </div>

        <div class="header-phone d-flex align-center">
            <img class="header-phone__img" src="icons/phone.svg" alt="Phone tube icon">

            <h4 class="header-phone__text">+38(095)-542-79-79</h4>
        </div>
    </div>
</template>


<script>
export default {
    data: () => ({
        menuLinks: [
            {
                title: 'Главная',
                path: '/',
                active: true,
            },
            {
                title: 'Щенки',
                path: '/',
                active: false,
            },
            {
                title: 'Выпускники',
                path: '/',
                active: false,
            },
            {
                title: 'Контакты',
                path: '/',
                active: false,
            },
        ],
    }),
}
</script>


<style lang="scss" scoped>
    .header {
        width: 1410px;
        margin: 0 auto;
        padding: 50px 0;

        &-logo {
            &__img {
                max-height: 60px;
                max-width: 60px;

                margin-right: 20px;
            }

            &__text {
                font-weight: 800;
                font-size: 36px;
            }
        }

        &-menu {
            &__link {
                font-size: 20px;
                font-weight: 500;

                margin-right: 50px;

                &:last-child {
                    margin-right: 0px;
                }

                &-active {
                    font-weight: 700;
                    padding-bottom: 16px;
                    border-bottom: 3px solid #1E1E1E;;
                }

                &:hover {
                    font-weight: 700;
                }
            }
        }

        &-phone {
            &__img {
                max-height: 33px;
                max-width: 33px;

                margin-right: 8px;
            }

            &__text {
                font-weight: 700;
                font-size: 24px;
            }
        }
    }
</style>