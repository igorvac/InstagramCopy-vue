<template>
  <ul>
    <li v-for="item in items" :key="item">
      <StoryItem
        v-bind:name="item.user"
        v-bind:pic="item.pic"
        v-bind:status="item.status"
      >
      </StoryItem>
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
          status: "unread",
        },
        {
          user: "Ananda",
          pic: "https://picsum.photos/id/1025/100/100",
          status: "unread",
        },
        {
          user: "Igor",
          pic: "https://picsum.photos/id/1005/100/100",
          status: "unread",
        },
        {
          user: "Ananda",
          pic: "https://picsum.photos/id/1025/100/100",
          status: "unread",
        },
        {
          user: "Igor",
          pic: "https://picsum.photos/id/1005/100/100",
          status: "read",
        },
        {
          user: "Ananda",
          pic: "https://picsum.photos/id/1025/100/100",
          status: "read",
        },
        {
          user: "Igor",
          pic: "https://picsum.photos/id/1005/100/100",
          status: "read",
        },
        {
          user: "Ananda",
          pic: "https://picsum.photos/id/1025/100/100",
          status: "read",
        },
        {
          user: "Igor",
          pic: "https://picsum.photos/id/1005/100/100",
          status: "read",
        },
        {
          user: "Ananda",
          pic: "https://picsum.photos/id/1025/100/100",
          status: "read",
        },
        {
          user: "Igor",
          pic: "https://picsum.photos/id/1005/100/100",
          status: "read",
        },
        {
          user: "Ananda",
          pic: "https://picsum.photos/id/1025/100/100",
          status: "read",
        },
        {
          user: "Igor",
          pic: "https://picsum.photos/id/1005/100/100",
          status: "read",
        },
        {
          user: "Ananda",
          pic: "https://picsum.photos/id/1025/100/100",
          status: "read",
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