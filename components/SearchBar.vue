<template>
    <div class="search-bar__container">
        <div class="input__container">
            <input type="text" placeholder="Search for an event">
        </div>
        <img src="../assets/images/line.png" class="line">
        <div class="category__container">
            <select name="Categories" id="category">
                <option>category</option>
                <option v-for="category in categories" :key="category.id" value="none">{{ category }}</option>

            </select>
        </div>

        <div class="search-button__container">
            <button class="search__button">Search</button>
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            categories: []
        }
    },

    created() {
        this.getCategories()
    },

    methods: {
        // use the events api to get categories
        getCategories() {
            const headers = {
                accept: {
                    'Content-Type': 'application/json',
                    'Access-Control-Allow-Origin': '*'
                }
            }
                fetch('https://rendezvous-events.onrender.com/events', headers)
                .then((res) => res.json())
                .then(data => { console.log(data); data.data.allEvents.forEach(event => {
                    if(!this.categories.includes(event.category)) this.categories.push(event.category)
                });})
        },
    }



}
</script>

<style scoped>
.search-bar__container {
    background-color: #fff;
    color: #432361;
    display: flex;
    gap: 16px;
    width: 600px;
    height: 100px;
    padding: 0px 24px;
    justify-content: space-between;
    align-items: center;
    border-radius: 20px;
}

.input__container input {
    border: none;
    outline: none;
    color: #4F4F4F;
    font-family: 'Gilroy-Regular ☞';
    font-size: 16px;
    font-style: normal;
    font-weight: 400;
    line-height: normal;
    text-align: center;
}

.line {
    width: 2px;
    height: 51px;
}

.category__container select {
    border: none;
    outline: none;
    color: #4F4F4F;
    font-family: 'Gilroy-Regular ☞';
    font-size: 16px;
    font-style: normal;
    font-weight: 400;
    line-height: normal;
}

.search__button {
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

@media screen and (max-width: 768px) {
    .search-bar__container {
        width: 420px;
        height: 70px;
    }
}

@media screen and (max-width: 480px) {
    .search-bar__container {
        /* flex-wrap: wrap; */
        width: 360px;
        /* height: 100px; */
        /* flex-direction: column; */
        padding-left: 12px;
        padding-right: 12px;
        gap: 20px;
    }

    .input__container input {
        text-align: left;
    }

    .search__button {
        display: none;
    }
}

@media screen and (max-width: 375px) {
    .search-bar__container {
        width: 330px;
        padding-left: 8px;
        padding-right: 8px;
    }

    .input__container input {
        text-align: center;
        font-size: 12px;
    }

    .category__container select {

        text-align: center;
        font-size: 12px;
    }
}

@media screen and (max-width: 320px) {
    .search-bar__container {
        width: 250px;
    }

    .input__container input {
        font-size: 12px;
    }

    .category__container select {
        font-size: 10px;
    }

}
</style>