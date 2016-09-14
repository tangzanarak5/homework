<template>
  <div id="app">
    <score :scoreleft = "scoreleft" :scoreright = "scoreright"></score>
    <point-left :oneleft = "oneleft" :twoleft = "twoleft" :threeleft = "threeleft" :downleft = "downleft" :scoreleft = "scoreleft"></point-left>
    <point-right :oneright = "oneright" :tworight = "tworight" :threeright = "threeright" :downright = "downright" :scoreright = "scoreright"></point-right>
  </div>
</template>

<script>
import Score from './components/Score'
import PointLeft from './components/PointLeft'
import PointRight from './components/PointRight'

export default {
  data () {
    return {
      scoreleft: 0,
      scoreright: 0
    }
  },
  components: {
    Score,
    PointLeft,
    PointRight
  },
  methods: {
    oneleft: function () {
      this.scoreleft = this.scoreleft + 1
    },
    twoleft: function () {
      this.scoreleft = this.scoreleft + 2
    },
    threeleft: function () {
      this.scoreleft = this.scoreleft + 3
    },
    downleft: function () {
      this.scoreleft = this.scoreleft - 1
    },
    oneright: function () {
      this.scoreright = this.scoreright + 1
    },
    tworight: function () {
      this.scoreright = this.scoreright + 2
    },
    threeright: function () {
      this.scoreright = this.scoreright + 3
    },
    downright: function () {
      this.scoreright = this.scoreright - 1
    }
  }
}
</script>

<style>
html {
  height: 100%;
}

body {
  display: flex;
  align-items: center;
  justify-content: center;
  height: 100%;
}

#app {
  color: #2c3e50;
  margin-top: -100px;
  max-width: 600px;
  font-family: Source Sans Pro, Helvetica, sans-serif;
  text-align: center;
}

#app a {
  color: #42b983;
  text-decoration: none;
}

.logo {
  width: 100px;
  height: 100px
}
</style>
