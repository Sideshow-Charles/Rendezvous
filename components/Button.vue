<template>
    <button class="button" :class="btnStyle"><nuxt-link to="#">
            <slot />
        </nuxt-link></button>
</template>

<script>
export default {
    // Using the button as a component to avoid repetition, which then leads to populating the codebase.
    props: {
        btnStyle: {
            type: String,
            default: ''
        }
    }
}
</script>

<style scoped>
.button {
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

@media screen and (max-width: 1080px) {
    .sign-up__button {
        display: none;
    }
}

@media screen and (max-width: 480px) {
    .search__button {
        display: none;
    }
}
</style>