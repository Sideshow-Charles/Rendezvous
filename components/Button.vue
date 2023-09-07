<template>
    <button class="button"><nuxt-link to="#">
            <slot/>
        </nuxt-link></button>
</template>

<script>
export default {

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
</style>