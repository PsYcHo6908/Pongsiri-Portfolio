<template>
  <div class="Background-B">
    <div class="profileImg">
      <img class="Img-about" src="../assets/Untitled-1.png" />
    </div>
    <div class="circle"></div>
  </div>
</template>
<script>
export default {}
</script>
<style>
.Background-B {
  background-color: black;
  height: 95vh;
  display: flex;
}
.profileImg {
    width: 45%;
}
img .Img-about {
  width: 100%;
  margin: 5% 5%;
}
.circle {
    position: relative;
    width: 25%;
    padding-bottom: 25%;
    background: rgb(255, 255, 255);
    border-radius: 50%;
    height: 25%;
    margin: 15% 0%;
}
</style>
