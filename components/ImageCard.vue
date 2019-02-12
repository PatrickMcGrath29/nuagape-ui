<template>
  <div class="image-card">
    <img v-bind:src="imageUrl">
    <div class="image-card__title"><h3>{{description}}</h3></div>
    <a v-bind:href="linkPath"></a>
  </div>
</template>

<script>
export default {
  name: 'ImageCard',
  props: ['imageUrl', 'linkPath', 'description']
}
</script>
<style>
@import '@/assets/styles/components/image_card.scss';
</style>
