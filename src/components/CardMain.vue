<template>
  <div>
    <img
      :src="comics.thumb"
      :alt="comics.series"
    >
    <div class="text">{{ comics.series.toUpperCase() }}
    </div>
  </div>
</template>

<script>
export default {
  name: 'CardMain',
  props: {
    comics: Object,
  },
};
</script>

<style lang="scss" scoped>

img {
  width: 90%;
  aspect-ratio: 1 / 1;
  object-fit: cover;
  object-position: 2px 5px;
}
.text {
  color: white;
}

</style>
