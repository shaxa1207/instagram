<template>
  <div class="container">
    <div class="row">
      <div class="col-8">
        <div class="wrapper-story">
          <ul class="story-list">
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
  .story-list {
    margin: 0;
    padding: 0;
    &__item {
      margin: 0 4px;
    }
  }
}
</style>
