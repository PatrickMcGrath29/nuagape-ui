<template>
  <footer
    role="contentinfo"
    :style="{'background-image': 'url(' + require('@/static/crossword.png') + ')'}"
  >
    <div class="container">
      <div class="footer-content">
        &copy; Agape Christian Fellowship 2019
      </div>
    </div>
  </footer>
</template>
<script>
export default {
  name: 'Footer'
}
</script>
