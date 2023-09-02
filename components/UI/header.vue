<template>
    <div class="main__header">
        <div class="logo__container">
            <img src="../../assets/app-logo.png" alt="app logo">
        </div>

        <ul class="nav__items__center">
            <li class="nav__item__center">Discover</li>
            <li class="nav__item__center">About us</li>
            <li class="nav__item__center">FAQs</li>
            <li class="nav__item__center">Contact us</li>
        </ul>

        <div class="nav__items__right">
            <li class="nav__item__right">Log in</li>
            <button class="sign-up__button">Sign up</button>
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
    font-family: 'Inter', sans-serif;
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
    font-family: 'Inter', sans-serif;
    margin: 0 24px
}

.sign-up__button {
    color: #FFF;
    font-family: Gilroy-SemiBold;
    font-size: 16px;
    font-style: normal;
    font-weight: 400;
    line-height: normal;
    border-radius: 10px;
    padding: 12px 24px;
    background: #783EAD;
    border: none;
}
</style>

