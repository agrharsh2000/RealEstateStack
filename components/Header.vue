<template>
  <div class="header-class">
    <div class="left">
      <h1 class="intro-h1">
        Let's build your <span><p></p></span> dream house
      </h1>

      <div class="button-container">
        <Button
          text="Find Property"
          @click="handleButtonClick"
          variant="primary"
        />
        <Button text="Explore" @click="handleButtonClick" variant="secondary" />
      </div>
      <div class="stacks-wrapper">
        <div class="stack">
          <span class="stack-heading">43K+</span>
          <span class="stack-description">Regular Customers</span>
        </div>
        <div class="stack">
          <span class="stack-heading">203K+</span>
          <span class="stack-description">Projects Completed</span>
        </div>
      </div>
      <div id="house-image" class="house">
        <img src="../assets/retro-house.jpg" />
      </div>
      <div class="house-rect"></div>
    </div>
    <div class="right"></div>
    <div class="review-card-holder">
      <ReviewCard />
    </div>
    <div class="circle">

    </div>
  </div>
</template>

<script setup>
import ReviewCard from "./data/review-card.vue";
</script>


<style scoped>
.circle{
  height: 100px;
  width: 100px;
  background: #fff;
  border-radius: 50%;
  position: absolute;
  right:15%;
  top:12rem;
  z-index: 20;
  box-shadow: 0px 0px 100px #ccc;
}
.review-card-holder{
  position: absolute;
  right:30%;
  z-index: 15;
}
.house-rect {
  position: absolute;
  height: 550px;
  width: 400px;
  transform: rotate(-30deg);
  border: #e8704d solid 2px;
  top: 10rem;
  right: 22rem;
  z-index: 5;
}
.house {
  z-index: 10;
  position: absolute;
  height: 650px;
  width: auto;
  top: 10rem;
  right: 22rem;
  transform: rotate(10deg);
}

.house img {
  height: 100%;
  width: 100%;
}

.intro-h1 {
  font-size: 64px;
  max-width: 400px;
  line-height: 105%;
}
.intro-h1 span p {
  height: 6px;
  width: 100%;
  background-color: #e8704d;
  display: inline-block;
}
.intro-h1 span {
  margin-top: 0px;
  max-height: 20px;
  width: 130px;
  display: inline-flex;
}

.header-class {
  margin-left: 40px;
}

.left {
  margin-top: 100px;
  margin-left: 26px;
  font-size: 40px;
}

h1 {
  text-align: left;
}

h1 span {
  display: block;
  margin-bottom: 20px;
}

.my-button {
  padding: 18px 36px;
  font-size: 20px;
  font-weight: 400;
  border-radius: 99px;
  border: none;
  transition: all 0.3s ease;
  cursor: pointer;
}

.my-button--primary {
  background-color: #000000;
  color: #ffffff;
}

.my-button:hover {
  background-color: #ffffff;
  color: #000000;
}

.my-button--secondary {
  background-color: #ffffff;
  color: #000000;
  padding-left: 50px;
  padding-right: 50px;
  margin-left: 10px;
  border: 1px solid;
}

.my-button:hover {
  background-color: #000000;
  color: #ffffff;
}

.stacks-wrapper {
  margin-top: 40px;
  display: flex;
  justify-content: space-between;
  gap: 10px;
  text-align: left;
  max-width: 300px;
}

.stack {
  display: flex;
  flex-direction: column;
  text-align: center;
}

.stack-heading {
  font-size: 40px;
  color: #ea6f4b;
  font-weight: 700;
}

.stack-description {
  font-size: 16px;
  max-width: 120px;
}
</style>
