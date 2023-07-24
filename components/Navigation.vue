<template>
<nav class="navigation">
    <div>
        <img src="../assets/logo.png" alt="Image" style="margin-left: 40px; width: 200px; height: 50px;">
    </div>
    <div class="nav-links">

        <nuxt-link :to="'/Home'" class="custom-link">Home</nuxt-link>
        <nuxt-link :to="'/Home'" class="custom-link">Buy</nuxt-link>
        <nuxt-link :to="'/Home'" class="custom-link">Sell</nuxt-link>
        <nuxt-link :to="'/Home'" class="custom-link">Contact us</nuxt-link>
    </div>
    <div class="button-container">
        <Button text="Sign up" @click="handleButtonClick" variant="primary" />
        <Button text="Log in" @click="handleButtonClick" variant="secondary" />
    </div>
</nav>
</template>

<script>
import Button from "./Button.vue";

export default {
    name: "Navigation",
    methods: {
        handleButtonClick() {
            console.log("Button Clicked");
        },
    },
};
</script>

<style scoped>
.navigation {
    padding-top: 36px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    font-family:"sans-serif"

}

.nav-links {
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 76px;
}

.custom-link {
    text-decoration: none;

    color: #18181A;
    font-weight: 500;
    font-size: 24px;
    line-height: 1.5;
    font-weight: 600;
}

.button-container {
    display: flex;
    justify-content: space-around;
    align-items: left;
    gap: 6px;
    margin-right: 70px;
}
</style>
