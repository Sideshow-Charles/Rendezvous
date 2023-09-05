<template>
    <footer class="footer__container">
        <footer class="footer__items__left">
            <footer class="footer__logo__container">
                <img src="../assets/images/footerlogo.png" alt="footer logo">
            </footer>
            <footer class="footer__item__left__text__container">
                <p class="footer__item__text__left">Your Personal Event Sherpa: Curating Awesome, One Click at a Time.</p>
            </footer>
        </footer>

        <footer class="footer__items__right">
            <div class="features">
                <p class="features__header">Feature</p>
                <ul class="features__items">
                    <li class="feature__item">Events Discovery</li>
                    <li class="feature__item">Ticketing</li>
                </ul>
            </div>

            <div class="company">
                <p class="company__header">Company</p>
                <ul class="company__items">
                    <li class="company__item">About</li>
                    <li class="company__item">FAQs</li>
                    <li class="company__item">Careers</li>
                    <li class="company__item">Support</li>
                </ul>
            </div>

            <div class="contact">
                <p class="contact__header">Contact us</p>
                <ul class="contact__items">
                    <li class="contact__item">info@events.com</li>
                    <li class="contact__item">+234 701 345 6789</li>
                    <li class="contact__item">Race Course, 8/9 Marina, Onikan, Lagos Lagos, 4aa Force Rd, Lagos Island
                        102273, Lagos</li>
                </ul>
            </div>
        </footer>
    </footer>
</template>

<script>
export default {

}
</script>

<style scoped>
.footer__container {
    background-color: #432361;
    padding: 64px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    /* gap: 350px; */
    /* overflow: hidden; */
}

.footer__logo__container img {
    width: 170px;
}

.footer__item__left__text__container {
    margin-top: 8px;
    width: 332px;
}

.footer__item__text__left {
    color: #FFF;
    font-family: 'Gilroy-Regular ☞';
    font-size: 16px;
    font-style: normal;
    font-weight: 400;
    line-height: 1.5;
}

.footer__items__right {
    display: flex;
    justify-content: space-between;
    align-items: flex-start;
    gap: 84px;
}

.features {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: flex-start;
    gap: 18px;
    width: 123px;
}

.features__header {
    color: #FFF;
    font-family: 'Gilroy-SemiBold ☞';
    font-size: 18px;
    font-style: normal;
    font-weight: 100;
    line-height: normal;
}

.feature__item {
    color: #FFF;
    font-family: 'Gilroy-Regular ☞';
    font-size: 16px;
    font-style: normal;
    font-weight: 400;
    line-height: normal;
    list-style: none;
    margin-bottom: 12px
}

.company {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: flex-start;
    gap: 18px;
    width: 91px;
}

.company__header {
    color: #FFF;
    font-family: 'Gilroy-SemiBold ☞';
    font-size: 18px;
    font-style: normal;
    font-weight: 100;
    line-height: normal;
}

.company__item {
    color: #FFF;
    font-family: 'Gilroy-Regular ☞';
    font-size: 16px;
    font-style: normal;
    font-weight: 400;
    line-height: normal;
    list-style: none;
    margin-bottom: 12px
}

.contact {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: flex-start;
    gap: 18px;
    width: 240px;
}

.contact__header {
    color: #FFF;
    font-family: 'Gilroy-SemiBold ☞';
    font-size: 18px;
    font-style: normal;
    font-weight: 100;
    line-height: normal;
}

.contact__item {
    color: #FFF;
    font-family: 'Gilroy-Regular ☞';
    font-size: 16px;
    font-style: normal;
    font-weight: 400;
    line-height: normal;
    list-style: none;
    margin-bottom: 12px
}

@media screen and (max-width: 968px) {
    .footer__container {
        flex-direction: column;
        align-items: flex-start;
        gap: 70px;
    }
}

@media screen and (max-width: 768px) {
    .footer__items__right {
        flex-direction: column;
        gap: 40px;
    }
}

@media screen and (max-width: 540px) {
    .footer__container {
        padding-left: 16px;
        padding-right: 16px;
    }
}

@media screen and (max-width: 280px) {
    .footer__item__left__text__container {
       width: 100%;

    }
}
</style>