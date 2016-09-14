<template>
  <div class="hello">
    <h1 class="h1">{{scoreleft}}
      <img src="http://www.uppic.org/thumb-EF07_57D97F31.jpg" border="0" width="100" height="100">
      {{scoreright}}</h1>
  </div>
</template>

<script>
export default {
  props: ['scoreleft', 'scoreright']
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.h1 {
  color: #111;
}
</style>
