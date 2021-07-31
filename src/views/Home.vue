<template>
  <link
    href="https://fonts.googleapis.com/icon?family=Material+Icons"
    rel="stylesheet"
  />
  <link
    href="https://fonts.googleapis.com/css?family=Material+Icons|Material+Icons+Outlined|Material+Icons+Two+Tone|Material+Icons+Round|Material+Icons+Sharp"
    rel="stylesheet"
  />

  <!-- 
  <div class="container">
    

  
    

    <Feed></Feed>
    
  <BottomMenu></BottomMenu>
  </div>
  
  -->
  <div class="head">
    <img src="@/assets/logo_ig.svg" alt="" />
    <span class="material-icons-outlined">add_box</span>
    <span class="material-icons">favorite_border</span>
    <span class="material-icons-outlined">question_answer</span>
  </div>
  <StoryBar></StoryBar>
  <Feed></Feed>
</template>

<script>
// @ is an alias to /src
//import HelloWorld from "@/components/HelloWorld.vue";

import StoryBar from "@/components/StoryBar.vue";
import Feed from "@/components/Feed.vue";

export default {
  name: "Home",
  components: {
    StoryBar,
    Feed,
  },
};
</script>

<style lang="scss">
@import "@/assets/variables.scss";

.container {
  width: 60rem;
  background-color: #ff0000;
}
.head {
  color: $gray;
  display: flex;
  align-items: center;
  padding: 1rem 0 0 0.5rem;
  //background-color: #ff0000;
  img {
    width: 6rem;
    margin-right: auto;
  }
  span {
    padding: 0.5rem;
  }
}
</style>
