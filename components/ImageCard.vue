<template>
  <div class="image-card">
    <img :src="imageUrl">
    <div class="image-card__title">
      <h3>{{ description }}</h3>
    </div>
    <a :href="linkPath" />
  </div>
</template>

<script>
export default {
  name: 'ImageCard',
  props: ['imageUrl', 'linkPath', 'description']
}
</script>
<style>
</style>
