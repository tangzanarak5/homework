<template>
    <button class="button" @click="oneleft">+1</button>
    <button class="button" @click="twoleft">+2</button>
    <button class="button" @click="threeleft">+3</button>
    <button class="button" @click="downleft" disabled ="{{scoreleft<=0}}">-1</button>
</template>

<script>
export default {
  props: ['oneleft', 'twoleft', 'threeleft', 'downleft', 'scoreleft']
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1 {
  color: #42b983;
}
.button {
    background-color: #008CBA; /* Green */
    border: none;
    color: white;
    text-align: center;
    text-decoration: none;
    display: inline-block;
    cursor: pointer;
}
</style>
