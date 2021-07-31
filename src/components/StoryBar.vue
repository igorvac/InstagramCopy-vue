<template>
  <ul>
    <li v-for="item in items" :key="item">
      <StoryItem v-bind:name="item.user" v-bind:pic="item.pic"> </StoryItem>
    </li>
  </ul>
</template>

<script>
// @ is an alias to /src
import StoryItem from "@/components/StoryItem.vue";

export default {
  name: "StoryBar",
  components: {
    StoryItem,
  },
  data() {
    return {
      items: [
        {
          user: "Igor",
          pic: "https://picsum.photos/id/1005/100/100",
        },
        {
          user: "Ananda",
          pic: "https://picsum.photos/id/1025/100/100",
        },
        {
          user: "Igor",
          pic: "https://picsum.photos/id/1005/100/100",
        },
        {
          user: "Ananda",
          pic: "https://picsum.photos/id/1025/100/100",
        },
        {
          user: "Igor",
          pic: "https://picsum.photos/id/1005/100/100",
        },
        {
          user: "Ananda",
          pic: "https://picsum.photos/id/1025/100/100",
        },
        {
          user: "Igor",
          pic: "https://picsum.photos/id/1005/100/100",
        },
        {
          user: "Ananda",
          pic: "https://picsum.photos/id/1025/100/100",
        },
        {
          user: "Igor",
          pic: "https://picsum.photos/id/1005/100/100",
        },
        {
          user: "Ananda",
          pic: "https://picsum.photos/id/1025/100/100",
        },
        {
          user: "Igor",
          pic: "https://picsum.photos/id/1005/100/100",
        },
        {
          user: "Ananda",
          pic: "https://picsum.photos/id/1025/100/100",
        },
        {
          user: "Igor",
          pic: "https://picsum.photos/id/1005/100/100",
        },
        {
          user: "Ananda",
          pic: "https://picsum.photos/id/1025/100/100",
        },
      ],
    };
  },
};
</script>


<style lang="scss" scoped>
@import "@/assets/variables.scss";

ul {
  display: flex;
  overflow: auto;
}
ul::-webkit-scrollbar {
  display: none;
}
</style>