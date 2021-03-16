<template>
  <div class="org">
    <NavBar></NavBar>
    <Form caption="Table"></Form>
  </div>
</template>

<script>
import NavBar from "@/components/NavBar.vue";
import Form from "@/components/Form.vue";

export default {
  components: {
    NavBar,
    Form
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
.org {
  height: 100vh;
  z-index: 100;
}
</style>
