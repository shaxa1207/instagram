<template>
  <div id="app">
    <main-header />
    <insta-story :stories="stories" />
  </div>
</template>

<script>
import MainHeader from "./components/mainHeader.vue";
import InstaStory from "./components/instaStory";

export default {
  data: function () {
    return {
      stories: [
        {
          image: "../assets/images/subscriber1.png",
        },
      ],
    };
  },
  components: {
    InstaStory,
    MainHeader,
  },
};
</script>
<style lang="scss">
body,
html,
#app {
  background-color: #fafafa;
}
</style>
