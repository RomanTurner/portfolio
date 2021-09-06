<template>
  <div class="decorative">
    <div class="avatar">
      <img alt="Vue logo" src="../../assets/profile_pic.png" />
    </div>
  </div>
  <div class="decorative-contact">
    <div class="contact-info">
      <a href="mailto: roman.nturner@gmail.com"
        ><Gmail class="icon" /> roman.nturner@gmail.com</a
      >
      <a href="https://github.com/RomanTurner"
        ><Linkedin class="icon" /> github.com/RomanTurner</a
      >
      <a href="https://www.linkedin.com/in/roman-turner/"
        ><Github class="icon" /> linkedin.com/in/roman-turner</a
      >
    </div>
  </div>
</template>
<script>
import { Linkedin } from "mdue";
import { Github } from "mdue";
import { Gmail } from "mdue";

export default {
  name: "App",
  components: {
    Linkedin,
    Github,
    Gmail,
  },
};
</script>
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
  text-align: left;
  flex-direction: column;
  background-color: #ebebeb;
  padding-left: 10px;
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
a {
  text-decoration: none;
  color: black;
}

a .icon {
  color: #77c9e7;
  text-decoration: none;
  font-size: 24px;
}
</style>
