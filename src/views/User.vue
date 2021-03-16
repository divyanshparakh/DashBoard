<template>
  <div class="usr">
    <NavBar></NavBar>
    <p>User</p>
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
.usr {
  height: 100vh;
  background-color: lightyellow;
}
</style>
