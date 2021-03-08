<template>
  <div>
    <nav class="navbar navbar-expand-md navbar-light bg-white shadow-sm">
      <router-link :to="{ name: 'home' }" class="navbar-brand">
          <img src="https://www.boolean.careers/images/misc/logo.png" alt="Boolean Careers">
      </router-link>
      <button
        class="navbar-toggler"
        data-toggle="collapse"
        data-target="#navbarCollapse"
      >
        <span class="navbar-toggler-icon"></span>
      </button>
      <div id="navbarCollapse" class="collapse navbar-collapse">
        <ul class="navbar-nav">
          <li class="nav-item">
            <router-link class="nav-link" :to="{ name: 'home' }">Home</router-link>
          </li>

          <li class="nav-item">
            <router-link class="nav-link" :to="{ name: 'about' }">About</router-link>
          </li>

          <li class="nav-item">
            <router-link class="nav-link" :to="{ name: 'contact' }">Contact us</router-link>
          </li>
        </ul>
      </div>
    </nav>

    <div class="container">
      <router-view></router-view>
    </div>

    <footer class="text-center mt-5">
      <router-link :to="{ name: 'contact' }">Contact us</router-link>
    </footer>
  </div>
</template>

<script>
export default {
  
}
</script>

<style scoped>
    .navbar-brand img {
        max-width: 150px;
    }
</style>