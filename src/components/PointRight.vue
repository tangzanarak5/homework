<template>
        <button class="button" @click="oneright">+1</button>
        <button class="button" @click="tworight">+2</button>
        <button class="button" @click="threeright">+3</button>
        <button class="button" @click="downright" disabled ="{{scoreright<=0}}">-1</button>
</template>

<script>
export default {
  props: ['oneright', 'tworight', 'threeright', 'downright', 'scoreright']
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1 {
  color: #42b983;
}
.button {
    background-color: #4CAF50; /* Green */
    border: none;
    color: white;
    text-align: center;
    text-decoration: none;
    display: inline-block;
    cursor: pointer;
}
</style>
