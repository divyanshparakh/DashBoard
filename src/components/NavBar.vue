<template>
  <div>
    <a><Wrapper class="Wrapper" @click="Show()"></Wrapper></a>
    <nav class="nav-links-small">
      <a class="immutable" href="/">
        C
        <img
          id="logo"
          rel="icon"
          src="https://cdn2.iconfinder.com/data/icons/coronavirus-15/1024/coronavirus-256.png"
        />
        vid
      </a>
      <menu class="sidebar">
        <Cross @click="Cross()"></Cross>
        <ul>
          <li><a href="/">Home</a></li>
          <li><a href="/organization-setup">Organization Setup</a></li>
          <li><a href="/user-setup">User Setup</a></li>
          <li><a href="/custom-user-setup">Custom User Setup</a></li>
        </ul>
      </menu>
    </nav>
    <nav class="nav-links">
      <ul>
        <li>
          <a class="immutable" href="/">
            C
            <img
              id="logo"
              rel="icon"
              src="https://cdn2.iconfinder.com/data/icons/coronavirus-15/1024/coronavirus-256.png"
            />
            vid
          </a>
        </li>
        <li><a href="/organization-setup">Organization Setup</a></li>
        <li><a href="/user-setup">User Setup</a></li>
        <li><a href="/custom-user-setup">Custom User Setup</a></li>
      </ul>
    </nav>
  </div>
</template>

<script>
import Wrapper from "@/components/NavigationBar/Wrapper.vue";
import Cross from "@/components/NavigationBar/Cross.vue";

export default {
  components: {
    Wrapper,
    Cross
  },
  props: {},
  data() {
    return {};
  },
  computed: {},
  methods: {
    Show() {
      document.querySelector(".sidebar").style.display = "flex";
    },
    Cross() {
      document.querySelector(".sidebar").style.display = "none";
    }
  },
  created() {},
  mounted() {}
};
</script>

<style lang="scss" scoped>
.nav-links {
  display: none;
}
.nav-links-small {
  background: #2a6a9a; /* fallback for old browsers */
  background-image: linear-gradient(
    to top right,
    #7d599d,
    #6261a2,
    #4566a1,
    #2a6a9a,
    #146c90,
    #146c90
  );
  background: -webkit-linear-gradient(
    to top,
    #7d599d,
    #6261a2,
    #4566a1,
    #2a6a9a,
    #146c90,
    #146c90
  ); /* Chrome 10-25, Safari 5.1-6 */
  box-shadow: 0 0 5px rgba(3, 47, 65, 1);
  height: 60px;
  display: flex;
  .immutable {
    display: flex;
    color: white;
    justify-content: center;
    font-size: 2em;
    position: absolute;
    font-family: "Lucida Console", Monaco, monospace;
    left: 2em;
    top: 0.5em;
    #logo {
      height: 1.4em;
      width: 1.4em;
      position: relative;
      top: -0.1em;
    }
  }
  .sidebar {
    background: #2a6a9a; /* fallback for old browsers */
    background-image: linear-gradient(
      to top,
      #7d599d,
      #6261a2,
      #4566a1,
      #2a6a9a,
      #146c90,
      #146c90
    );
    background: -webkit-linear-gradient(
      to top,
      #7d599d,
      #6261a2,
      #4566a1,
      #2a6a9a,
      #146c90,
      #146c90
    ); /* Chrome 10-25, Safari 5.1-6 */
    justify-content: center;
    flex-flow: column nowrap;
    position: absolute;
    right: 0;
    width: 50vw;
    height: 100vh;
    box-shadow: 0 0 5px rgba(3, 47, 65, 1);
    overflow: hidden;
    ul {
      font-size: 1em;
      display: block;
      list-style-type: none;
      li {
        position: relative;
        margin: 1em;
        a {
          color: white;
          text-decoration: none;
        }
      }
    }
  }
}
$breakpoint-tablet: 768px;
@media (min-width: $breakpoint-tablet) {
  .Wrapper,
  .nav-links-small {
    display: none;
  }
  .nav-links {
    background: #2a6a9a; /* fallback for old browsers */
    background-image: linear-gradient(
      to top,
      #7d599d,
      #6261a2,
      #4566a1,
      #2a6a9a,
      #146c90,
      #146c90
    );
    background: -webkit-linear-gradient(
      to top,
      #7d599d,
      #6261a2,
      #4566a1,
      #2a6a9a,
      #146c90,
      #146c90
    ); /* Chrome 10-25, Safari 5.1-6 */
    display: block;
    ul {
      font-size: 1.5em;
      display: flex;
      justify-content: center;
      li {
        margin: 1em;
        display: flex;
        align-items: center;
        flex-wrap: wrap;
        .immutable {
          text-decoration: none;
          display: flex;
          justify-content: center;
          font-size: 2em;
          position: absolute;
          font-family: "Lucida Console", Monaco, monospace;
          left: 2em;
          &:hover {
            img {
              transform: scale(1.2);
            }
          }
          #logo {
            height: 1.4em;
            width: 1.4em;
            position: relative;
            top: -0.1em;
          }
        }
        a {
          margin-left: 2em;
          color: white;
          text-decoration: none;
        }
      }
    }
  }
}
</style>
