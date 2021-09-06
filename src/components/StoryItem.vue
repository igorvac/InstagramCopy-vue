<template>
  <div class="item">
    <div v-bind:class="status">
      <img v-bind:src="pic" alt="" />
      <div class="bgwhite"></div>
    </div>
    <p class="">
      {{ name }}
    </p>
  </div>
</template>



<script>
export default {
  props: {
    name: {
      type: String,
      required: true,
    },
    pic: {
      type: String,
      required: true,
    },
    status: {
      type: String,
      required: true,
    },
  },
};
</script>

<style lang="scss" scoped>
@import "../assets/variables";
@import "../assets/baseStyle";

p {
  font-size: $fontSM;
}

.item {
  display: flex;
  flex-direction: column;
  align-items: center;
  margin: 0.5rem;
}

$img-siz: 3rem;

img {
  width: $img-siz;
  border: 0.2rem solid #ffffff;
  border-radius: $img-siz;
}

.unread {
  display: flex;
  align-items: center;
  justify-content: center;
  border-radius: $img-siz;
  padding: 0.1rem;
  background-image: linear-gradient(to left, #bb2288, #ffaa66);
  margin-bottom: 0.5rem;
  .bgwhite {
    display: none;
  }
}
//background-image: linear-gradient(to left, #bb2288, #ffaa66);
.read {
  display: flex;
  align-items: center;
  justify-content: center;
  border-radius: $img-siz;
  padding: 0.1rem;
  background-image: linear-gradient(to left, #cccccc, #cccccc);
  margin-bottom: 0.5rem;
  .bgwhite {
    position: absolute;
    width: 3.1rem;
    height: 3.1rem;
    border-radius: $img-siz;
    background-color: #ffffff;
  }
  img {
    z-index: 1;
    opacity: 0.6;
  }
}
</style>

