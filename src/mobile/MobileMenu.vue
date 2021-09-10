<template>
  <div class="content" :style="{ backgroundImage: 'url(' + bgImage + ')' }">
    <Avatar />
    <header class="top">
      <hr />
      <h1>R O M A N</h1>
      <h1>T U R N E R</h1>
      <h4>FULLSTACK DEVELOPER</h4>
    </header>
    <hr />
    <section class="main">
      <article>
        <h3 class="article-title">About me<span class="dot">.</span></h3>
        <p>
          I am a JavaScript and Sushi enthusiast with a soft spot for Ruby and
          Musubi. I derive purpose from creation and I have a passion for making
          tools that can make your life easier. I am a community builder with
          ten years of experience working with small teams in production. I
          believe everyone has a unique skill or vision and I love seeing it
          piece together.
        </p>
      </article>
      <hr />
      <article>
        <h3 class="article-title">Projects<span class="dot">.</span></h3>
        <h4>Flavorites</h4>
        <img :src="flavoritesImage" alt="meal planning interface on laptop" />
        <p class="links">
          <em>GitHub: </em>
          <a
            href="https://github.com/RomanTurner/flavorites-frontend"
            target="_blank"
            >Frontend</a
          >
          |
          <a
            href="https://github.com/RomanTurner/flavorites-backend"
            target="_blank"
            >Backend</a
          >
          <em>— 3 Minute Run Through- </em>
          <a
            href="https://www.loom.com/share/1ff5f9ed13a6472eab40e2822f1b08d9"
            target="_blank"
            >Demo</a
          >
          | <em>Full Walkthrough - </em>
          <a href="https://www.youtube.com/watch?v=-6AuczkTqu4" target="_blank"
            >Demo</a
          >
        </p>
        <p class="subtitle">
          Web application for assigning meal plans as a feature for an existing
          recipe website.
        </p>
        <ul class="details">
          <li>
            Composed authenticated routing using React Router and JSON Web
            Tokens.
          </li>
          <li>
            Instituted Drag and Drop functionality, for a real nice user
            experience. Check out the demo.
          </li>
          <li>
            Leveraged React functional components and the modern Redux Toolkit
            for state management.
          </li>
          <li>
            Used Kimurai to scrape data from a dynamic website and seed a
            postgreSQL database.
          </li>
        </ul>
      </article>
      <hr />
      <article>
        <h3 class="article-title">Contact Me<span class="dot">.</span></h3>
        <p>
          Use any of my contact links to get in touch for any opportunities.
          View website on a larger screen for more content.
        </p>
      </article>
      <hr />
    </section>
  </div>
</template>

<script>
import flavoritesImage from "@/mobile/assets/flavorites-laptop.gif";
import bgImage from "@/mobile/assets/intro-bg.png";
import Avatar from "../components/navigation/Avatar.vue";
export default {
  name: "MobileMenu",
  components: { Avatar },
  data() {
    return {
      flavoritesImage,
      bgImage,
    };
  },
};
</script>

<style scoped>
.content {
  background-attachment: fixed;
  background-size: 100%;
  background-repeat: no-repeat;
}
.main {
  display: flex;
  flex-direction: column;
  align-items: center;
}
.top {
  padding-bottom: 10px;
  width: 100%;
  height: 190px;
  text-align: left;
}
.top h1 {
  font-size: 3em;
  margin: 0;
}
img {
  max-width: 300px;
  height: auto;
}
.top hr {
  max-width: 100px;
  margin: 0px;
  border-top: 8px solid #77c9e7;
  border-left: 3px solid #77c9e7;
  border-right: 3px solid #77c9e7;
  border-bottom: 5px solid black;
}
hr {
  border: solid 1px #ebebeb;
  border-top: 5px solid #77c9e7;
  border-bottom: 1px solid black;
  width: 85%;
}
p {
  text-align: left;
  background-color: rgb(255, 255, 255, 0.5);
}
h3 {
  background: #77c9e7;
  color: #ffffff;
}

.article-title {
  padding-left: 5px;
  text-align: left;
  font-size: 48px;
}
.dot {
  font-size: 64px;
}
article p {
  margin: 0;
}

ul {
  text-align: left;
  margin: 0;
}
</style>
