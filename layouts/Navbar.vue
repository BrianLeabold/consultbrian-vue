<template>
  <footer class="fixed bottom-0 w-full">
    <nav class="bg-blue-800 border border-blue-800 text-white">
      <ul class="flex justify-around text-center">
        <nuxt-link
          class="nav-item items-center w-1/5 cursor-pointer hover:bg-white hover:text-blue-800 active:bg-white active:text-blue-800 text-center"
          to="/"
        >
          <li class>
            Home
            <br />
            <i class="fas fa-home"></i>
          </li>
        </nuxt-link>
        <nuxt-link
          class="nav-item w-1/5 cursor-pointer hover:bg-white hover:text-blue-800 active:bg-white active:text-blue-800 text-center"
          to="/services"
        >
          <li class>
            Services
            <br />
            <i class="fas fa-list-ul"></i>
          </li>
        </nuxt-link>
        <nuxt-link
          class="nav-item w-1/5 cursor-pointer hover:bg-white hover:text-blue-800 active:bg-white active:text-blue-800 text-center"
          to="/photos"
        >
          <li class>
            Photos
            <br />
            <i class="fa fa-camera"></i>
          </li>
        </nuxt-link>
        <nuxt-link
          class="nav-item w-1/5 cursor-pointer hover:bg-white hover:text-blue-800 active:bg-white active:text-blue-800 text-center"
          to="/news"
        >
          <li class>
            What's New
            <br />
            <i class="fa fa-newspaper"></i>
          </li>
        </nuxt-link>
        <nuxt-link
          class="nav-item w-1/5 cursor-pointer hover:bg-white hover:text-blue-800 active:bg-white active:text-blue-800 text-center"
          to="/contact"
        >
          <li class>
            Contact
            <br />
            <i class="far fa-envelope"></i>
          </li>
        </nuxt-link>
      </ul>
    </nav>
  </footer>
</template>
<script>
export default {
  name: 'Navbar'
}
</script>
<style scoped>
a.nav-item {
  transition: background-color 0.5s linear;
}
.nuxt-link-exact-active {
  background: white;
}
</style>