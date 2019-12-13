<template>
  <div class="loader_container">
    <div class="loader" data-perc="0.83"></div>
    <div class="loader_content text-center">
      <div class="loader_title brus">creativity brus</div>
      <div class="loader_subtitle">Odio vestibulum est mattis.</div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    percent: {
      type: Number,
      default: 0
    }
  }
};
</script>

<style scoped>
.loaders {
  margin-top: 98px;
}
.loader_container {
  width: 25%;
  height: 265px;
  float: left;
  padding-bottom: 70px;
}
.loader {
  width: 195px;
  height: 195px;
  margin: 0 auto;
  background: transparent;
}
.loader_content {
  position: absolute;
  left: 50%;
  bottom: 0;
  -webkit-transform: translateX(-50%);
  -moz-transform: translateX(-50%);
  -ms-transform: translateX(-50%);
  -o-transform: translateX(-50%);
  transform: translateX(-50%);
  font-size: 18px;
  font-weight: 500;
  color: #232323;
  white-space: nowrap;
  text-align: center;
}
.loader_title {
  font-size: 16px;
  font-weight: 700;
  color: #100f3a;
  text-transform: uppercase;
  line-height: 0.75;
}
.loader_subtitle {
  font-size: 14px;
  font-weight: 500;
  color: #7a798c;
  margin-top: 12px;
}
</style>