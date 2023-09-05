<template>
    <div class="search-bar__container">
        <div class="input__container">
            <input type="text" placeholder="Search for an event">
        </div>
        <img src="../assets/images/line.png" class="line">
        <div class="category__container">
            <select name="Categories" id="category">
                <option value="none">Categories</option>
                <option>All</option>
                <option>Comedy</option>
                <option>Religious</option>
                <option>Tech</option>
                <option>Health</option>
                <option>Fitness</option>
                <option>Education</option>
            </select>
        </div>

        <div class="search-button__container">
            <button class="search__button">Search</button>
        </div>
    </div>
</template>

<script>
export default {

}
</script>

<style scoped>
.search-bar__container {
    background-color: #fff;
    color: #432361;
    display: flex;
    gap: 16px;
    width: 660px;
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
        width: 460px;
        height: 70px;
    }
}

@media screen and (max-width: 480px) {
    .search-bar__container {
        /* flex-wrap: wrap; */
        width: 370px;
        /* height: 100px; */
        /* flex-direction: column;
        padding: 16px 0; */
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
    width: 350px;
  }
}
</style>