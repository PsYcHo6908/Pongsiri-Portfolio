<template>
  <div class="Background-W">
    <div class="Frame-contract">
      <img class="Img-contract" src="../assets/contract-img.jpg" />
    </div>
    <div class="box-contract">
      <div class="box-icon">
        <img class="Icon" src="../assets/email.png" />
        <div class="text-contact">Pongsiri5770@gmail.com</div>
      </div>
      <div class="box-icon">
        <img class="Icon" src="../assets/call.png" />
        <div class="text-contact">092-282-5770</div>
      </div>

    </div>
  </div>
</template>
<script>
export default {}
</script>
<style>
.Background-W {
  background-color: rgb(255, 255, 255);
  height: 95vh;
  display: flex;
}
.Frame-contract {
  width: 50%;
}
img.Img-contract {
  border-radius: 50px;
  width: 70%;
  margin: 5% 5%;
}
.box-contract {
  width: 50%;
}
.box-icon {
    display: flex;
    gap: 5%;
    margin-top: 5%;
}
img.Icon {
  width: 10%;
}
.text-contact {
    margin-top: 3%;
}
</style>
