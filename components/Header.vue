<template>
    <div class="main__header" :class="headerStyle">
        <div class="logo__container">
            <nuxt-link to="/"><img src="../assets/images/app-logo.png" alt="app logo"></nuxt-link>
        </div>


        <ul class="nav__items__center">
            <li class="nav__item__center"><nuxt-link to="#">Discover</nuxt-link></li>
            <li class="nav__item__center"><nuxt-link to="#">About us</nuxt-link></li>
            <li class="nav__item__center"><nuxt-link to="#">FAQs</nuxt-link></li>
            <li class="nav__item__center"><nuxt-link to="#">Contact us</nuxt-link></li>
        </ul>

        <div class="nav__items__right">
            <li class="nav__item__right"><nuxt-link to="#">Log in</nuxt-link></li>

            <!-- Button Component -->
            <Button btnStyle="sign-up__button">Sign up</Button>
            <!-- End of Button Component -->

            <!-- navigation menu icon -->
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
import Button from "../components/Button"
export default {
    components: {
        Button
    },
    // Using the header as a component to avoid repetition, which then leads to populating the codebase.
    props: {
        headerStyle: {
            type: String,
            default: ''
        }
    }

}
</script>

<style scoped>
.main__header {
    align-items: center;
    background: hsla(0, 0%, 100%, .6);
    border-radius: 20px;
    display: flex;
    justify-content: space-between;
    margin: 0 64px;
    padding: 12px 24px;
    position: relative;
    top: 50px;
    z-index: 1000;
}

/* Header Styling For The Alternative Header */
.view-event__header {
    background: transparent;
    position: static;
    margin-top: 40px;
    margin-bottom: 46px;
}

/* End of Header Styling For The Alternative Header */

.logo__container {
    margin: 0 24px;
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
    font-weight: 400;
    margin: 0 24px
}

.nav__items__right {
    display: flex;
    align-items: center;
    margin: 0 24px
}

.nav__item__right {
    display: flex;
    font-family: 'Gilroy-Bold ☞';
    color: #432361;
    margin: 0 24px
}

.hamburger__menu__icon {
    display: none;
    cursor: pointer;
}

@media screen and (min-width: 1600px) {
    .main__header {
        width: 1312px;
        margin: 0 auto;
    }

    .view-event__header {
        margin-top: 40px;
        margin-bottom: 46px;
    }
}

@media screen and (max-width: 1080px) {

    .nav__items__center,
    .nav__item__right {
        display: none;
    }
    .hamburger__menu__icon {
    display: block;
}
}


@media screen and (max-width: 980px) {
    .main__header {
        width: 80%;
        margin: 0 auto;
    }

    .view-event__header {
        padding-top: 50px;
    }
}

@media screen and (max-width: 768px) {
    .view-event__header {
        width: auto;
        margin-left: 0;
        margin-right: 0;
        padding-left: 0;
        padding-right: 0;
    }
}

@media screen and (max-width: 540px) {
    .main__header {
        width: 90%;
        margin: 0 auto;
        padding-left: 8px;
        padding-right: 8px;
    }

    .view-event__header {
        width: auto;
        margin-left: 0;
        margin-right: 0;
        padding-left: 0;
        padding-right: 0;
    }

    .logo__container img {
        width: 100px;
    }
}

@media screen and (max-width: 480px) {

    .logo__container img {
        width: 100px;
    }
}
</style>

