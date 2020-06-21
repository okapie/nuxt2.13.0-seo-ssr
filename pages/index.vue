<template>
  <div class="container">
    <div>
      <header class="content-logos">
        <logo />
        <span class="plus">+</span>
        <VuesaxLogo />
      </header>
      <h1 class="title">
        Nuxt.js + Vuesax
      </h1>
      <h2 class="subtitle">
        <a href="https://vuesax.com/">Vuesax</a> is a framework of ui components
        for <a href="https://vuejs.org/">Vuejs</a>, It was created to make new
        interfaces that have a new trend and are visually beautiful
      </h2>
      <div class="links">
        <h3 class="h3">
          Vuesax
        </h3>
        <div class="buttons-wrapper">
          <vs-button
            onclick="window.open('https://vuesax.com/','_blank')"
            color="success"
            type="filled"
          >
            Documentation
          </vs-button>
          <vs-button
            onclick="window.open('https://discordapp.com/invite/9dsKtvB','_blank')"
            color="success"
            type="filled"
          >
            Discord
          </vs-button>
          <vs-button
            onclick="window.open('https://github.com/lusaxweb/vuesax','_blank')"
            color="success"
            type="filled"
          >
            GitHub
          </vs-button>
        </div>
      </div>
      <div class="links">
        <h3 class="h3">
          Nuxt.js
        </h3>
        <div class="buttons-wrapper">
          <vs-button
            onclick="window.open('https://nuxtjs.org/','_blank')"
            color="success"
            type="filled"
          >
            Documentation
          </vs-button>
          <vs-button
            onclick="window.open('https://github.com/nuxt/nuxt.js','_blank')"
            color="success"
            type="filled"
          >
            GitHub
          </vs-button>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Logo from "~/components/Logo.vue";
import VuesaxLogo from "~/components/VuesaxLogo.vue";

export default {
  components: {
    Logo,
    VuesaxLogo,
  },
  head() {
    return {
      title: "OGP TAG TEST",
      meta: [
        {
          hid: "description",
          name: "description",
          content: "Here's meta description",
        },
        { hid: "og:type", property: "og:type", content: "article" },
        {
          hid: "og:title",
          property: "og:title",
          content: "TOP | OGP TAG TEST",
        },
        {
          hid: "og:description",
          property: "og:description",
          content: "Here's meta description.",
        },
        {
          hid: "og:url",
          property: "og:url",
          content: "http://www.example.com",
        },
        {
          hid: "og:image",
          property: "og:image",
          content: "http://www.example.com/ogp_dummy.png",
        },
      ],
    };
  },
};
</script>

<style>
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  font-family: "Quicksand", "Source Sans Pro", -apple-system, BlinkMacSystemFont,
    "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
  display: block;
  font-weight: 300;
  font-size: 55px;
  color: #35495e;
  letter-spacing: 1px;
  text-transform: capitalize;
  margin: 25px 0;
}

.subtitle {
  font-weight: 300;
  font-size: 1.1rem;
  color: #526488;
  word-spacing: 2px;
  padding-bottom: 15px;
  max-width: 600px;
}

.subtitle a {
  font-weight: 500;
  color: inherit;
}

.links {
  padding-top: 15px;
  margin-bottom: 20px;
}

.content-logos {
  display: flex;
  align-items: center;
  justify-content: center;
  min-width: 500px;
}

.plus {
  font-size: 2.5rem;
  margin: 15px;
  color: #35495e;
}

.h3 {
  font-family: "Quicksand", "Source Sans Pro", -apple-system, BlinkMacSystemFont,
    "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
  font-weight: 400;
  margin: 10px;
}

.buttons-wrapper {
  display: flex;
  justify-content: center;
}
</style>
