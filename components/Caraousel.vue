<template>
<div class="company-card-container">
    <div class="company-card">
        <img src="../assets/C1.png" class="company-card-image" alt="" />
    </div>
    <div class="company-card">
        <img src="../assets/C2.png" class="company-card-image" alt="" />
    </div>
    <div class="company-card">
        <img src="../assets/C3.png" class="company-card-image" alt="" />

    </div>
    <div class="company-card">
        <img src="../assets/C4.png" class="company-card-image" alt="" />

    </div>
</div>
</template>

<script>
export default {
    name: "Caraousel",
}
</script>

<style>

.company-card-container { 
  position: relative;
  width: 92%;
  margin: auto;
  height: 10vw;
  display: flex;
  margin-top: 260px;
  margin-bottom: 120px;
  justify-content: space-between;
}
.company-card {
  margin-top: 70px;
  position: relative;
  min-width: calc(100% / 5 - 10px);
  width: calc(100% / 5 - 10px);
  height: 100%;
  border-radius: 5px;
  overflow: hidden;
  
}
.company-card-image{
  width: 90%;
  height: 90%;
  object-fit: cover;
}
</style>
