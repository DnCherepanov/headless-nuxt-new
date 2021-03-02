<template>
  <nav class="nav">
        <nuxt-link exact to="/">
          <app-icon></app-icon>
        </nuxt-link>
    <div class="external">
      <ul>
        <li>
          <nuxt-link to="/about">About</nuxt-link>
        </li>
        <li>
          <nuxt-link to="/archive">Archive</nuxt-link>
        </li>
        <li>
          <nuxt-link to="/contact">Contact</nuxt-link>
        </li>
        <select v-model="$colorMode.preference">
          <option value="system">System</option>
          <option value="light">Light</option>
          <option value="dark">Dark</option>
          <option value="sepia">Sepia</option>
        </select>
      </ul>
      <a
        href="https://github.com/sahkyo/nuxt-transition"
        target="_blank"
        rel="noopener noreferrer"
      >
        <svg viewBox="0 0 24 24" width="24" height="24">
          <use href="@/assets/img/github.svg#github" />
        </svg>
      </a>
      <a
        href="https://link.medium.com/Zl1yg9KfVab"
        target="_blank"
        rel="noopener noreferrer"
      >
        <svg viewBox="0 0 24 24" width="24" height="24">
          <use href="@/assets/img/medium.svg#medium" />
        </svg>
      </a>
    </div>
  </nav>
</template>

<script>
import AppIcon from "@/components/AppIcon.vue";

export default {
  components: {
    AppIcon
  }
};
</script>

<style lang="scss" scoped>
.nav {
  padding: 1.3em 34px;
  a {
    opacity: 0.8;
    &:hover {
      opacity: 1;
    }
  }
}

ul {
  padding-left: 0;

  li {
    display: inline-block;
    margin-right: 30px;
  }
}
</style>
