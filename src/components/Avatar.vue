<template>
  <div>
    <figure class="avatar">
      <img :src="src" :alt="alt" :width="size" :height="size" />
    </figure>
    <p>username</p>
  </div>
</template>

<script>
export default {
  name: "Avatar",
  props: {
    src: {
      type: String,
      default:
        "https://pbs.twimg.com/profile_images/1346076211521449991/CAIzJaNA_400x400.jpg",
    },
    alt: {
      type: String,
    },
    size: {
      type: Number,
    },
  },
};
</script>

<style scoped>
.avatar {
  display: inline-flex;
  padding: 2px;
  border-radius: 50%;
  background: linear-gradient(
    219deg,
    rgba(184, 63, 140, 1) 0%,
    rgba(237, 158, 90, 1) 100%
  );
}

.avatar img {
  border-radius: 999px;
}
</style>
