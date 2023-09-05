<template>
    <div class="main__header">
        <div class="logo__container">
            <img src="../assets/images/app-logo.png" alt="app logo">
        </div>


        <ul class="nav__items__center">
            <li class="nav__item__center"><nuxt-link to="#">Discover</nuxt-link></li>
            <li class="nav__item__center"><nuxt-link to="#">About us</nuxt-link></li>
            <li class="nav__item__center"><nuxt-link to="#">FAQs</nuxt-link></li>
            <li class="nav__item__center"><nuxt-link to="#">Contact us</nuxt-link></li>
        </ul>

        <div class="nav__items__right">
            <li class="nav__item__right"><nuxt-link to="#">Log in</nuxt-link></li>
            <button class="sign-up__button"><nuxt-link to="#">Sign up</nuxt-link></button>

            <!-- navigation menu -->
            <svg xmlns="http://www.w3.org/2000/svg" x="0px" y="0px" width="50" height="20" viewBox="0 0 50 50"
                style="fill:#432361;" class="hamburger__menu__icon">
                <path
                    d="M 0 7.5 L 0 12.5 L 50 12.5 L 50 7.5 Z M 0 22.5 L 0 27.5 L 50 27.5 L 50 22.5 Z M 0 37.5 L 0 42.5 L 50 42.5 L 50 37.5 Z">
                </path>
            </svg>
        </div>
    </div>
</template>

<script>
export default {

}
</script>

<style scoped>
.main__header {
    border-radius: 20px;
    background: rgba(255, 255, 255, 0.60);
    z-index: 1000;
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 12px 24px;
    position: relative;
    top: 50px;
    margin: 0 62px;
}

.logo__container img {
    width: 170px;
}

.nav__items__center {
    display: flex;
    align-items: center;
}

.nav__item__center {
    display: flex;
    font-family: 'Gilroy-Bold ☞';
    color: #432361;
    font-style: normal;
    font-weight: 700;
    margin: 0 24px
}

.nav__items__right {
    display: flex;
    align-items: center;
}

.nav__item__right {
    display: flex;
    font-family: 'Gilroy-Bold ☞';
    color: #432361;
    margin: 0 24px
}

.sign-up__button {
    color: #FFF;
    font-family: 'Gilroy-Light ☞';
    font-size: 16px;
    font-style: normal;
    font-weight: 400;
    line-height: normal;
    border-radius: 10px;
    padding: 12px 24px;
    background: #783EAD;
    border: none;
}

.hamburger__menu__icon {
    display: none;
    cursor: pointer;
}

@media screen and (max-width: 980px) {

    .nav__items__center,
    .nav__item__right,
    .sign-up__button {
        display: none;
    }

    .hamburger__menu__icon {
        display: block;
    }
}

@media screen and (max-width: 540px) {
    .main__header {
        margin-left: 16px;
        margin-right: 16px;
    }
}

@media screen and (max-width: 480px) {
    .logo__container img {
        width: 100px;
    }
}
</style>

