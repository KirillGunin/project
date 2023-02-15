<template>
  <header>
    <div class="navbar">
      <div class="container">
        <div class="navbar-content">
          <div class="logo">Logo</div>
          <ul class="navbar-list">
            <li class="navbar-item" v-for="link in links" :key="link.title">
              <NuxtLink
                class="navbar-link"
                :title="link.title"
                :to="link.url"
                >{{ link.title }}</NuxtLink
              >
            </li>
          </ul>
        </div>
      </div>
    </div>
  </header>
</template>

<script>
export default {
  data() {
    return {
      links: [
        {
          title: "Home",
          url: "/",
        },
        {
          title: "About",
          url: "/about",
        },
        {
          title: "Войти",
          url: "/admin",
        },
      ],
    };
  },
};
</script>

<style lang="scss">
.navbar-link {
  &.nuxt-link-exact-active {
    color: #06414b;
  }
}
</style>
