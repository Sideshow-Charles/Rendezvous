<template>
  <div class="landing__page">
    <!-- Landing Page Hero Section -->
    <div class="hero__section">
      <!-- Header Component -->
      <Header></Header>
      <!-- End of Header Component -->
      <div class="hero__items__container">
        <p class="hero__text">Ready to Rock? Discover the Hottest Events Here – Your Calendar's New Best Friend!</p>
        <!-- Seach Bar Component -->
        <SearchBar></SearchBar>
        <!-- End of Search Bar Component -->
      </div>
    </div>
    <!-- End of Landing Page Hero Section-->

    <!--Events Container -->
    <section class="events__container">
      <!-- Events Header -->
      <section class="events__header__container">
        <p class="events__header__text__left">Trending events</p>
        <p class="events__header__text__right">View all trending events <svg width="16" height="17" viewBox="0 0 16 17"
            fill="none" xmlns="http://www.w3.org/2000/svg">
            <rect width="16" height="16" transform="translate(0 0.5)" fill="white" style="mix-blend-mode:multiply" />
            <path d="M5 3.5V4.5H11.295L3 12.795L3.705 13.5L12 5.205V11.5H13V3.5H5Z" fill="#432361" />
          </svg> </p>
      </section>
      <!-- End of Events Header -->

      <!-- Event Cards -->
      <div class="event__card__container">

        <!-- Single Event -->
        <div class="event__card">
          <div class="event__image">
            <img src="../assets/images/ISWIS.png" alt="Event Image">
          </div>
          <div class="event__details">
            <p class="event__name">ISWIS Live show</p>
            <div class="event__date__and__time">
              <p class="event__date">Sun, Oct 3rd</p>
              <p class="event__time">6pm</p>
            </div>
            <p class="event__description">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor
              incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco
              laboris
              nisi ut aliquip ex ea commodo consequat.</p>
          </div>
        </div>

        <!-- End of Single Event -->

        <!-- Single Event -->
        <div class="event__card">
          <div class="event__image">
            <img src="../assets/images/NATIV5.png" alt="Event Image">
          </div>
          <div class="event__details">
            <p class="event__name">ISWIS Live show</p>
            <div class="event__date__and__time">
              <p class="event__date">Sun, Oct 3rd</p>
              <p class="event__time">6pm</p>
            </div>
            <p class="event__description">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor
              incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco
              laboris
              nisi ut aliquip ex ea commodo consequat.</p>
          </div>
        </div>
        <!-- End of Single Event -->

        <!-- Single Event -->
        <div class="event__card">
          <div class="event__image">
            <img src="../assets/images/UNPROVOKED.png" alt="Event Image">
          </div>
          <div class="event__details">
            <p class="event__name">ISWIS Live show</p>
            <div class="event__date__and__time">
              <p class="event__date">Sun, Oct 3rd</p>
              <p class="event__time">6pm</p>
            </div>
            <p class="event__description">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor
              incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco
              laboris
              nisi ut aliquip ex ea commodo consequat.</p>
          </div>
        </div>
        <!-- End of Single Event -->
      </div>
      <!-- End of Events Card-->
    </section>
    <!-- End of Event Container-->

    <!-- Discover Section -->
    <section class="discover__container">
      <section class="discover__text__container">
        <p class="discover__text">Discover a World of Events Tailored Just for You.</p>
        <button class="CTA-discover__events">View all events</button>
      </section>
      <section class="discover__images__container">
        <img src="../assets/images/online.png" alt="discover online images">
        <img src="../assets/images/physical.png" alt="discover online images">
        <img src="../assets/images/hybrid.png" alt="discover online images">
      </section>
    </section>
    <!-- End of Discover Section -->

    <!-- Footer Component -->
    <Footer></Footer>
    <!-- End of Footer Component -->
  </div>
</template>

<script>
import Header from "../components/Header";
import SearchBar from "../components/SearchBar";
import Footer from "../components/Footer";
export default {
  components: {
    Header,
    SearchBar,
    Footer
  }
}
</script>
<style scoped>
.hero__section {
  background-image: url("../assets/images/hero-image.png");
  background-size: cover;
  background-repeat: no-repeat;
  background-color: lightgray;
  background-position: 50%;
  height: 640px;
}

.hero__items__container {
  display: flex;
  justify-content: space-between;
  gap: 121px;
  margin: 350px 64px 0 64px;
}

.hero__text {
  color: #fff;
  font-family: 'Gilroy-Bold ☞';
  width: 531px;
  font-size: 32px;
  font-style: normal;
  font-weight: 400;
  line-height: normal;
  z-index: 999;
}

.events__container {
  margin-top: 64px;
}

.events__header__container {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin: 0 64px;
}

.events__header__text__left {
  color: #000;
  font-family: 'Gilroy-Medium ☞';
  font-size: 32px;
  font-style: normal;
  font-weight: 400;
  line-height: normal;
}

.events__header__text__right {
  color: #432361;
  font-family: 'Gilroy-Medium ☞';
  font-size: 16px;
  font-style: normal;
  font-weight: 400;
  line-height: normal;
}

.event__card__container {
  display: flex;
  gap: 24px;
  align-items: center;
  margin: 47px 64px 100px 64px;
}

.event__card {
  width: 421px;
  height: 488px;
  border-radius: 10px;
  border: 1px solid #E0E0E0;
  background: #FFF;
}

.event__image img {
  width: 421px;
  height: 240px;
}

.event__details {
  margin: 24px 24px 33px 24px;
}

.event__name {
  margin-bottom: 4px;
  color: #000;
  font-family: 'Gilroy-Medium ☞';
  font-size: 16px;
  font-style: normal;
  font-weight: 400;
  line-height: normal;

}

.event__date__and__time {
  margin-top: 4px;
  display: flex;
  gap: 8px;
  color: #000;
  font-family: 'Gilroy-Regular ☞';
  font-size: 14px;
  font-style: normal;
  font-weight: 400;
  line-height: normal;
}

.event__description {
  margin-top: 16px;
  color: #000;
  font-family: 'Gilroy-Light ☞';
  font-size: 14px;
  font-style: normal;
  font-weight: 400;
  line-height: 1.5;
}

.discover__container {
  margin: 227px 64px 123px 64px;
  display: flex;
  gap: 92px;
}

.discover__text {
  color: #000;
  font-family: 'Gilroy-SemiBold ☞';
  font-size: 32px;
  font-style: normal;
  font-weight: 400;
  line-height: normal;
  width: 393px;
  margin: 48px 0 24px 0;
}

.CTA-discover__events {
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
  cursor: pointer;
}

.discover__images__container {
  display: flex;
  flex-wrap: wrap;
  gap: 25px;
}

.discover__images__container img {
  width: 400px;
  height: 240px;
}
</style>