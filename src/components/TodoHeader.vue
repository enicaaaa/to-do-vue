<script setup>
import { RouterLink } from 'vue-router';
</script>

<template>
    <header>
        <nav class="container">
            <div class="branding">
                <img src="../assets/Vue_Logo_Black.png" alt="">
                <h1>Vue Todos</h1>
            </div>
            <ul class="nav-routes">
                <RouterLink id="home-route" to="/">Home</RouterLink>
                <RouterLink id="meetings-route" to="/meetings">Meetings</RouterLink>
                <RouterLink id="about-route" to="/about">About</RouterLink>
            </ul>
        </nav>
    </header>
</template>


<style lang="scss" scoped>
header {
  background-color: #f1f1f1;
  nav {
    display: flex;
    align-items: center;
    padding: 25px 16px;

    .branding {
      display: flex;
      align-items: center;
      gap: 8px;
      img {
        max-width: 50px;
      }

      h1 {
        font-size: 24px;
      }
    }

    .nav-routes {
      display: flex;
      flex: 1;
      justify-content: flex-end;
      gap: 19px;
      list-style: none;

      a {
        text-decoration: none;
        color: inherit;
      }
    }
  }

  #home-route:hover {
    color: #41b080 !important;
    font-weight: bold;
  }

  #meetings-route:hover {
    color: #41b080 !important;
    font-weight: bold;
  }

  #about-route:hover {
    color: #41b080 !important;
    font-weight: bold;
  }

  .router-link-exact-active {
    color: #41b080 !important;
    font-weight: bold;
}
}
</style>