<template>
  <div class="review-card">
    <div class="review-card-images">
      <div class="review-card-image" style="left: 2rem">
        <img src="../../assets/users/p1.jpg" alt="user name for pic 1" />
      </div>
      <div class="review-card-image" style="left: 4rem">
        <img src="../../assets/users/p2.jpg" alt="user name for pic 2" />
      </div>
      <div class="review-card-image" style="left: 6rem">
        <img src="../../assets/users/p3.jpg" alt="user name for pic 3" />
      </div>
      <div class="review-card-image" style="left: 8rem">
        <img src="../../assets/users/p4.jpg" alt="user name for pic 4" />
      </div>
      <div class="review-card-image">
        <img src="../../assets/users/p5.jpg" alt="user name for pic 5" />
      </div>
    </div>
    <p>Check reviews</p>
  </div>
</template>
  
  <script>
</script>
  
  <style scoped>
.review-card {
  height: 50px;
  border-radius: 200px;
  width: 250px;
  background: #fff;
  padding: 0rem 1rem;
  display: flex;
  align-content: center;
  justify-content: space-between;
  align-items: center;
  box-shadow: 10px 0 40px #aaa;
}
.review-card p {
  font-size: 0.8rem;
  width:4rem
}
.review-card-images {
  display: flex;
  height: 40px;
  position: relative;
}
.review-card-image {
  position: absolute;
  border-radius: 50%;
  height: 40px;
  width: 40px;
  overflow: hidden;
  object-fit: cover;
  object-position: center;
  display: flex;
  align-items: center;
  background: #fff;
}

.review-card-image img {
  height: 35px;
  width: 35px;
  overflow: hidden;
  object-fit: cover;
  border-radius: 50%;
}
</style>
  