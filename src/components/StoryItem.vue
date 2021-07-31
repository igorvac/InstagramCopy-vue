<template>
  <div class="item">
    <img v-bind:src="pic" alt="" />
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
  },
};
</script>

<style lang="scss" scoped>
@import "../assets/variables";
@import "../assets/baseStyle";

p {
  font-size: $fontSM;
}

$img-siz: 3rem;

img {
  width: $img-siz;
  margin-bottom: 0.5rem;
  border-radius: $img-siz;
}

.item {
  display: flex;
  flex-direction: column;
  align-items: center;
  margin: 0.5rem;
}
</style>

