<template>
  <div class="wrapper">
    <div class="hamburger">
      <div class="first"></div>
      <div class="second"></div>
      <div class="third"></div>
    </div>
  </div>
</template>

<script>
export default {
  components: {},
  props: {},
  data() {
    return {};
  },
  computed: {},
  methods: {},
  created() {},
  mounted() {}
};
</script>

<style lang="scss" scoped>
.wrapper {
  position: absolute;
  top: 0px;
  right: 0px;
}

.hamburger {
  width: 60px;
  height: 60px;
  background: #146c90;
  cursor: pointer;
  position: relative;
  border-radius: 5px;
}

.hamburger > div {
  position: absolute;
  height: 7px;
  background: #fff;
  transition: width 0.3s ease;
  border-radius: 5px;
}

.first {
  width: 50px;
  top: 25px;
  left: 8px;
  transform: rotate(45deg);
}

.second {
  width: 50px;
  top: 25px;
  left: 8px;
  transform: rotate(-45deg);
}

.hamburger:active div {
  width: 0px;
  transition: width 0.4s ease;
}
</style>
