<template>
  <div class="top">
    <img src="https://picsum.photos/id/1062/50/50" alt="" />
    <h2>Igor</h2>
    <h2 class="text_click1">Follow</h2>
    <p class="text_click2">...</p>
  </div>

  <div class="post">
    <img src="https://picsum.photos/500/300" alt="" />
    <span class="material-icons">favorite_border</span>
    <span class="material-icons">chat_bubble_outline</span>
    <span class="material-icons-outlined"> send </span>
    <span class="material-icons">bookmark_border</span>
  </div>

  <div class="comment-bar">
    <ul>
      <li>
        <img src="https://picsum.photos/id/1062/50/50" alt="" />
      </li>
      <li>
        <img src="https://picsum.photos/id/1062/50/50" alt="" />
      </li>
      <li>
        <img src="https://picsum.photos/id/1062/50/50" alt="" />
      </li>
    </ul>
    <p>Liked by <span class="user">José</span></p>
  </div>
  <ul class="comments">
    <li>
      <p>
        <span class="user">user</span>
        <span
          >Lorem ipsum, dolor sit amet consectetur adipisicing elit. Error
          dolore suscipit odio, mollitia ducimus perspiciatis perferendis
          aliquid optio quaerat.
        </span>
      </p>
    </li>
  </ul>
</template>

<script>
export default {
  props: {},
};
</script>

<style lang="scss" scoped>
@import "@/assets/variables.scss";

$margins: 0.5rem;
$imgSize: 1.8rem;
$imgSizeSM: 1.2rem;

.user {
  font-weight: bold;
}
.top {
  display: flex;
  align-items: center;
  margin: $margins;
  h2 {
    margin-left: $margins;
    font-size: $fontMD;
    font-weight: bold;
  }

  img {
    $imgSize: 1.8rem;
    width: $imgSize;
    border-radius: $imgSize;
  }

  :last-child {
    margin-left: auto;
  }
}
.post {
  display: flex;
  flex-wrap: wrap;
  img {
    width: 100%;
  }
  span {
    padding: 0.3rem;
    color: $gray;
  }
  :last-child {
    margin-left: auto;
  }
}
.comment-bar {
  display: flex;
  flex-direction: row;
  align-items: center;
  ul {
    display: flex;
    flex-direction: row;
  }
  li {
    margin-right: -1rem;
    img {
      margin: 0.2rem;
      border-radius: $imgSize;
      border-color: #ffffff;
      border-style: solid;
      width: $imgSizeSM;
      border-width: 2px;
    }
  }
  p {
    margin-left: 1rem;
    font-size: $fontSM;
  }
}

.comments {
  margin-top: 0.2rem;
  margin-left: 0.3rem;
  p {
    font-size: $fontSM;
  }
}
</style>