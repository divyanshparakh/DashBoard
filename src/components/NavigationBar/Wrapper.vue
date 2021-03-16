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
  background: #2a6a9a;
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
  width: 45px;
  top: 10px;
  left: 8px;
}

.second {
  width: 30px;
  top: 25px;
  left: 8px;
}

.third {
  width: 40px;
  top: 40px;
  left: 8px;
}

.hamburger:hover div {
  width: 45px;
  transition: width 0.3s ease;
}
</style>
