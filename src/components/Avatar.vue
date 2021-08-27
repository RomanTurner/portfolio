<template>
  <div class="decorative">
    <div class="avatar">
      <img alt="Vue logo" src="../assets/profile_pic.png" />
    </div>
  </div>
  <div class="decorative-contact">
    <div class="contact-info">
      <span>Contact Info</span>
      <span>Contact Info</span>
      <span>Contact Info</span>
    </div>
  </div>
</template>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.decorative {
  background: linear-gradient(180deg, #ffffff 65%, #77c9e7 50%);
  padding-left: 20px;
}
.decorative-contact {
  background: #77c9e7;
  padding-left: 20px;
}
.contact-info {
  display: flex;
  flex-direction: column;
  background-color: #ebebeb;
}
.avatar {
  display: flex;
  justify-content: center;
  height: 100%;
  width: 100%;
  background: linear-gradient(180deg, #ffffff 50%, #ebebeb 50%);
}
img {
  width: 250px;
  object-fit: cover;
  border-radius: 50%;
}
</style>
