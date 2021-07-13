<template>
  <div class="container">
    <div class="row">
      <div class="col-7">
        <div class="wrapper-story">
          <ul class="story-list d-flex align-items-center">
            <li
              class="story-list__item"
              v-for="(element, index) in stories"
              :key="index"
            >
              <img :src="element.image" alt="" />
            </li>
          </ul>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "instaStory",
  props: {
    stories: {
      type: Array,
      default: () => {
        [];
      },
    },
  },
};
</script>

<style lang="scss" scoped>
ul li {
  list-style-type: none;
}
.wrapper-story {
  background: #fff;
  border: 1px solid #dbdbdb;
  border-radius: 3px;
  margin-bottom: 24px;
  padding: 16px 0;
  margin-top: 30px;
  width: 100%;
  .story-list {
    margin: 0;
    padding: 0 12px;
    &__item {
      margin: 0 8px;
      background: linear-gradient(108.03deg, #c7059a -15.49%, #dd0e44 118.71%);
      border-radius: 50%;
      width: 64px;
      height: 64px;
      position: relative;
      cursor: pointer;
      img {
        box-sizing: border-box;
        width: 60px;
        height: 60px;
        object-fit: cover;
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);
        border: 2px solid #fff;
        border-radius: 50%;
      }
    }
  }
}
</style>
