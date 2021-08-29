<template>
  <section class="projects">
    <h2>Technical Projects</h2>
    <article class="project">
      <h3 class="title">Flavorites</h3>
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
          Composed authenticated routing using React Router and JSON Web Tokens.
        </li>
        <li>
          Instituted Drag and Drop functionality, for a real nice user
          experience. Check out the demo.
        </li>
        <li>
          Leveraged React functional components and the modern Redux Toolkit for
          state management.
        </li>
        <li>
          Used Kimurai to scrape data from a dynamic website and seed a
          postgreSQL database.
        </li>
      </ul>
      <Collapsable />
    </article>
    <article class="project">
      <h3 class="title">CollegeReco</h3>
      <p class="links">
        <em>Website: </em>
        <a href="https://collegereco.com/" target="_blank"
          >https://collegereco.com/</a
        >
      </p>
      <p class="subtitle">College recommendation web application.</p>
      <p class="details">
        Created the frontend on React, working with a Data Scientist colleague
        that created and trained a data model hosted on a Python Flask app.
        Great experience working with different tech fields.
      </p>
      <Collapsable />
    </article>
    <article class="project">
      <h3 class="title">Dungeon Master’s ToolBox</h3>
      <p class="links">
        <em>GitHub: </em>
        <a href="https://github.com/RomanTurner/dms-toolbox/" target="_blank"
          >Frontend</a
        >
        |
        <a
          href="https://github.com/RomanTurner/dms-toolbox/tree/main/backend"
          target="_blank"
          >Backend</a
        >
      </p>
      <p class="subtitle">
        Intuitive management system for roleplayers. Worked closely with another
        fullstack RoR / React developer.
      </p>
      <ul class="details">
        <li>
          Designed custom controllers on Rack middleware, not using Rails, to
          manage user requests. Link to code.
        </li>
        <li>Utilized polymorphic associations across data models.</li>
        <li>Constructed the frontend using ‘legacy’ React class components.</li>
      </ul>
      <Collapsable />
    </article>
    <article class="project">
      <h3 class="title">MarKit Meals</h3>
      <p class="links">
        <em>Website: </em>
        <a href="https://markitmeals.com/" target="_blank"
          >https://markitmeals.com/</a
        >
      </p>
      <p class="subtitle">Seattle based meal-kit ecommerce site.</p>
      <ul class="details">
        <li>Customized Shopify UI/UX to maximize visitor conversion.</li>
      </ul>
      <Collapsable />
    </article>
    <article class="project">
      <h3 class="title">Raw, Blogging Application</h3>
      <p class="links">
        <em>GitHub: </em>
        <a
          href="https://github.com/RomanTurner/raw-blog-frontend"
          target="_blank"
          >Frontend</a
        >
        |
        <a
          href="https://github.com/RomanTurner/raw-blog-backend/"
          target="_blank"
          >Backend</a
        >
      </p>
      <p class="subtitle">
        Blogging application to harbor the random and raw thoughts of a user
        base.
      </p>
      <ul class="details">
        <li>
          Demonstrated security practices with hashing/salting encryption and
          tokenization.
        </li>
        <li>
          Maintained PostgreSQL database with full dynamic CRUD actions using
          RESTful routing practices.
        </li>
      </ul>
      <Collapsable />
    </article>
  </section>
</template>

<script>
import Collapsable from "../basic-components/Collapsable.vue";
export default {
  components: { Collapsable },
};
</script>

<style scoped>
section {
  text-align: left;
}
p {
  margin: 0;
}
ul {
  margin: 0;
}
</style>
