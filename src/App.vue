<template>
  <div id="app">
    <main-header />
    <insta-story :stories="stories" />
    <new-post :posts="posts" />
  </div>
</template>

<script>
import MainHeader from "./components/mainHeader.vue";
import InstaStory from "./components/instaStory";
import NewPost from "./components/newPost";

export default {
  data: function () {
    return {
      stories: [
        {
          id: 0,
          image: require("@/assets/images/subscriber1.png"),
        },
        {
          id: 1,
          image: require("@/assets/images/subscriber2.png"),
        },
        {
          id: 2,
          image: require("@/assets/images/subscriber3.png"),
        },
        {
          id: 3,
          image: require("@/assets/images/subscriber4.png"),
        },
        {
          id: 5,
          image: require("@/assets/images/subscriber2.png"),
        },
        {
          id: 6,
          image: require("@/assets/images/postimg4.jpg"),
        },
        {
          id: 7,
          image: require("@/assets/images/postimg2.jpg"),
        },
        {
          id: 8,
          image: require("@/assets/images/postimg3.jpg"),
        },
      ],
      posts: [
        {
          id: 0,
          image: require("@/assets/images/postimg4.jpg"),
        },
        {
          id: 1,
          image: require("@/assets/images/postimg2.jpg"),
        },
        {
          id: 2,
          image: require("@/assets/images/postimg3.jpg"),
        },
        {
          id: 3,
          image: require("@/assets/images/postimg1.png"),
        },
      ],
    };
  },
  components: {
    NewPost,
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
