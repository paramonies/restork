<template>
  <div class="content">
    <div class="img">
      <img :src="'/landing/' + image" />
    </div>
    <div class="title">
      {{ title }}
    </div>
    <div class="desc">
      {{ desc }}
    </div>
    <div class="wrapBtn">
      <b-button variant="primary" size="lg">Зарегестрироваться</b-button>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    image: {
      type: String,
      default: null
    },
    title: {
      type: String,
      default: null
    },
    desc: {
      type: String,
      default: null
    }
  }
}
</script>

<style lang="scss" scoped>
.content {
  display: flex;
  flex-direction: column;
  .img {
    padding: 70px 0 25px 0;
    @media (max-width: 767px) {
      padding: 0 0 25px 0;
    }
  }
  .title {
    padding-bottom: 25px;
    font-family: Montserrat;
    font-size: 20px;
    line-height: 26px;
    font-weight: 500;
    color: #000000;
    @media (max-width: 767px) {
      font-size: 16px;
      line-height: 20px;
    }
  }
  .desc {
    padding-bottom: 25px;
    font-family: Montserrat;
    font-size: 14px;
    line-height: 20px;
    font-weight: 400;
    color: #000000;
    @media (max-width: 767px) {
      font-size: 12px;
      line-height: 18px;
    }
  }
  .wrapBtn {
  }
}
</style>
