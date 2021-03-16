<template>
  <div class="custusr">
    <NavBar></NavBar>
    <p>CustomUser</p>
  </div>
</template>

<script>
import NavBar from "@/components/NavBar.vue";

export default {
  components: {
    NavBar
  },
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
.custusr {
  height: 100vh;
  background-color: lightyellow;
}
</style>
