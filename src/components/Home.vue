<template>
<div class="body">
  <div class="container">
    <Card name="MEME" icon="meme.png" address="0xFcACcCf880F274596c5d33A2d1f5705839ab4eF7"></Card>
    <Card name="KOBE" icon="kobe.png" address=""></Card>
    <Card name="CAT" icon="cat.png" address="0x1cABA43BE99e299f1d886D74e63C770C96cEd296"></Card>
    <Card name="NASA" icon="nasa.png" address="0x4dA588BcB861533B8e2e5b2E3140029Ce628cB06"></Card>
  </div>
  <div class="intro">
    <p>Umemeverse aims to do more meme token airdrops, you can claim any coin you want in this site. </p>
    <p>And if you are a project founder and want to do airdrop to your community without spending your own gas,</p>
  you can contact us via <el-link type="primary" class="email">umemeverse.com@gmail.com</el-link> , submit your token information, send us your token and rules.
  </div>
</div>
</template>

<script>
import Card from './Card'
export default {
    name: 'Stake',
    data() {
        return {
            balance: 0,
            amount: 0
        }
    },
    components: {
      Card
    },
    methods: {
        changeMethod: function (value) {
            this.method = value
        }
    },
    computed: {
        unit: function () {
            return this.method === 1 ? 'Num' : 'M'
        }
    }
}
</script>

<style scoped>
.body {
  width: 100%;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}

.container {
  width: 95%;
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  -webkit-box-align: center;
  align-items: center;
  align-content: center;
  flex: 1 1 0%;
  overflow: hidden auto;
  z-index: 1;
  padding: 20px 16px 16px;
}

.intro {
  color: #ffffff;
  font-size: 24px;
}

.email {
  font-size: 26px;
  line-height: 20px;
  font-weight: 500;
}
</style>
