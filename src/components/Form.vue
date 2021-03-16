<template>
  <div>
    <table>
      <caption>
        {{
          caption
        }}
      </caption>
    </table>
  </div>
</template>

<script>
export default {
  components: {},
  props: ["caption"],
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
table {
  background: no-repeat
    url("https://img.freepik.com/free-photo/empty-wooden-table-with-smoke-float-up-dark-background_68495-135.jpg?size=626&ext=jpg");
  background-size: cover;
  background-blend-mode: lighten;
  height: 900px;
  width: 900px;
  margin: auto;
  margin-top: 80px;
  margin-bottom: 100px;
  border-image: url("../assets/f0.gif") 25% repeat;
  caption {
    font-size: 2em;
    font-weight: 800;
  }
}
</style>
