<template>
  <header class="container py-3 d-flex justify-content-between align-items-center">
    <div class="logo">
      <img src="/img/dc-logo.png" alt="Logo DC">
    </div>
    <nav>
      <ul class="d-flex gap-3">
        <a :class="{active: link.current}" v-for="link in navbar" :href="link.url">
          <li>{{ link.text }}</li>
        </a>
      </ul>
    </nav>
  </header>
</template>

<script>
import { links } from '../data/data.js'

export default {
  name: "app-header",
  data() {
    return {
      navbar: links
    }
  }
}
</script>

<style lang="scss" scoped>
@mixin activelink {
  text-underline-offset: 63px;
      text-decoration: underline 6px #0282f9;
      color:#0282f9;
}

nav {
  a {
    text-decoration: none;
    list-style: none;
    padding: 0;
    margin: 0;
    color: #464646;
    font-weight: 700;
    text-transform: uppercase;

    &:hover {
      @include activelink;
    }
  }
}

.active {
  @include activelink;
}




</style>