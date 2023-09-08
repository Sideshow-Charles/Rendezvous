<template>
  <div id="landing__page">
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

    <section class="landing__page__body">

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

          <p v-if="err" class="error">Unable to get events, Please contact support</p>

          <!-- Single Event -->
          <nuxt-link :to="'/event/' + event.id" v-for="event in events" :key="event.id" class="event__card">
            <div class="event__image">
              <img :src=event.imageUrl alt="Event Image">
            </div>
            <div class="event__details">
              <p class="event__name">{{ event.title }}</p>
              <div class="event__date__and__time">
                <p class="event__date">{{ event.date }}</p>
                <p class="event__time">{{ event.time }}</p>
              </div>
              <p class="event__description">{{ event.description }}</p>
              <nuxt-link :to="'/event/' + event.id" class="event__link">View details <svg width="16" height="17"
                  viewBox="0 0 16 17" fill="none" xmlns="http://www.w3.org/2000/svg">
                  <rect width="16" height="16" transform="translate(0 0.5)" fill="white"
                    style="mix-blend-mode:multiply" />
                  <path d="M5 3.5V4.5H11.295L3 12.795L3.705 13.5L12 5.205V11.5H13V3.5H5Z" fill="#432361" />
                </svg></nuxt-link>
            </div>
          </nuxt-link>
        </div>
        <!-- End of Events Card-->
      </section>
      <!-- End of Event Container-->

      <!-- Discover Section -->
      <section class="discover__container">
        <section class="discover__text__container">
          <p class="discover__text">Discover a World of Events Tailored Just for You.</p>
          <Button>View all events</Button>
        </section>
        <section class="discover__images__container">
          <img src="../assets/images/online.png" alt="discover online images">
          <img src="../assets/images/physical.png" alt="discover online images">
          <img src="../assets/images/hybrid.png" alt="discover online images">
        </section>
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
import Button from "../components/Button";
export default {
  components: {
    Header,
    SearchBar,
    Footer,
    Button
  },

  data() {
    return {
      events: [],
      err: ''
    }
  },

  created() {
    //call the function to get all events as soon as the page is rendered
    this.getEvents()
  },

  methods: {
    //fetch all events
    getEvents() {
      const headers = {
        accept: {
          'Content-Type': 'application/json',
          'Access-Control-Allow-Origin': '*'
        }
      }

      fetch('https://rendezvous-events.onrender.com/events', headers)
        .then(res => res.json())
        .then(data => { console.log(data); this.events = data.data.allEvents })
        .catch((error) => {
          console.log(error);
          this.err = error 
        });
    }
  }
}
</script>
<style scoped>
#landing__page {
  overflow-x: hidden;
}

.hero__section {
  background-image: linear-gradient(rgba(0, 0, 0, 0.527), rgba(0, 0, 0, 0.5)), url("../assets/images/hero-image.png");
  background-size: cover;
  background-repeat: no-repeat;
  background-color: lightgray;
  position: absolute;
  top: 0%;
  bottom: 0%;
  left: 0%;
  right: 0%;
  height: 800px;
}

.hero__items__container {
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 100px;
  margin: 450px 64px 82px 64px;
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

.landing__page__body {
  max-width: 90rem;
  margin: 0 auto;
}

.events__container {
  margin-top: 850px;
}

.events__header__container {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin: 0 64px;
}

.error {
  color: red;
  font-family: 'Gilroy-Medium ☞';
  font-size: 24px;
  margin-top: 50px;
  margin-bottom: 0;
  margin-left: auto;
  margin-right: auto;
  text-align: center;
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
  align-items: flex-start;
  margin: 47px 64px 100px 64px;
  justify-content: space-between;
  flex-wrap: wrap;
}

.event__card {
  width: 410px;
  /* height: 448px; */
  border-radius: 10px;
  border: 1px solid #E0E0E0;
  background: #FFF;
}

.event__image img {
  width: 410px;
  height: 240px;
}

.event__details {
  margin: 24px 24px 33px 24px;
}

.event__name {
  margin-bottom: 8px;
  color: #000;
  font-family: 'Gilroy-Medium ☞';
  font-size: 16px;
  font-style: normal;
  font-weight: 400;
  line-height: normal;

}

.event__date__and__time {
  margin-top: 8px;
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
  margin-bottom: 24px;
  height: 80px;
  overflow: hidden;
  text-overflow: ellipsis;
}

.event__link {
  color: #432361;
  font-family: 'Gilroy-Regular ☞';
  font-size: 14px;
  font-style: normal;
  font-weight: 400;
  line-height: normal;
}

.discover__container {
  margin: 150px 64px 123px 64px;
  display: flex;
  justify-content: space-between;
  gap: 60px;
}

.discover__text__container {
  margin-top: 24px;
}

.discover__text {
  color: #000;
  font-family: 'Gilroy-SemiBold ☞';
  font-size: 32px;
  font-style: normal;
  font-weight: 400;
  line-height: normal;
  width: 393px;
  margin-top: 128px;
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
  margin-top: 24px;
  background: #783EAD;
  border: none;
  cursor: pointer;
}

.discover__images__container {
  display: flex;
  /* flex-flow: column wrap; */
  flex-wrap: wrap;
  gap: 25px;
}

.discover__images__container img {
  width: 410px;

  /* height: 240px; */
}

/* Media Queries */

@media screen and (max-width: 1100px) {
  .hero__items__container {
    flex-direction: column;
    justify-content: center;
    align-items: center;
    margin-top: 200px;
    gap: 30px;
    margin-left: auto;
    margin-right: auto;
  }

  .hero__text {
    /* width: 100%; */
    font-size: 38px;
  }
}

@media screen and (max-width: 968px) {

  .event__card,
  .event__image img {
    width: 100%;
  }

  .discover__container {
    flex-direction: column;
  }

  .discover__text__container {
    flex-direction: column;
    margin-left: 16px;
    margin-right: 16px;
  }

  .discover__images__container {
    margin-left: 16px;
    margin-right: 16px;
    flex-direction: row;
    flex-wrap: wrap;
  }

  .discover__images__container img {
    width: 45%;
    height: auto;
  }
}

@media screen and (max-width: 768px) {
  .events__header__text__left {
    font-size: 18px;
  }

  .events__header__text__right {
    font-size: 16px;
  }

  .discover__text {
    width: 320px;
    font-size: 24px;
  }

}

@media screen and (max-width: 540px) {

  /* .hero__items__container {
    margin: 0 auto;
  } */
  .hero__text {
    width: 450px;
    /* margin-left: 16px;
    margin-right: 16px; */
  }

  .events__header__container {
    flex-direction: column;
    align-items: flex-start;
    gap: 16px;
    margin-left: 16px;
    margin-right: 16px;
  }

  .event__card__container {
    margin-left: 16px;
    margin-right: 16px;
  }

  .event__card,
  .event__image img {
    width: 100%;
  }

  .discover__container {
    margin-left: 8px;
    margin-right: 8px;
  }

  /* .discover__text__container {
    margin-left: 16px;
    margin-right: 16px;
  } */

  .discover__images__container img {
    width: 100%;
  }
}

@media screen and (max-width: 480px) {

  .hero__items__container {
    margin-left: 16px;
    margin-right: 16px;
  }

  .hero__text {
    width: 100%;
    font-size: 30px;
  }

  .discover__text {
    width: 100%;
  }
}
</style>