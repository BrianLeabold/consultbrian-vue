<template>
  <footer class="fixed bottom-auto w-full">
    <nav class="bg-blue-800 border border-blue-800 text-white">
      <ul class="flex justify-around text-center">
        <nuxt-link
          class="nav-item align-middle items-center w-1/5 cursor-pointer hover:bg-white hover:text-blue-800 active:bg-white active:text-blue-800 text-center"
          to="/"
        >
          <li class="h-8 w-8 mt-1">
            <font-awesome-icon :icon="{ prefix: 'fa', iconName: 'home'}" />
          </li>Home
        </nuxt-link>
        <nuxt-link
          class="nav-item w-1/5 cursor-pointer hover:bg-white hover:text-blue-800 active:bg-white active:text-blue-800 text-center"
          to="/services"
        >
          <li class="h-8 w-8 mt-1">
            <font-awesome-icon :icon="{ prefix: 'fa', iconName: 'list-ul' }" />
          </li>Services
        </nuxt-link>
        <nuxt-link
          class="nav-item w-1/5 cursor-pointer hover:bg-white hover:text-blue-800 active:bg-white active:text-blue-800 text-center"
          to="/photos"
        >
          <li class="h-8 w-8 mt-1">
            <font-awesome-icon :icon="{ prefix: 'fa', iconName: 'camera' }" />
          </li>Photos
        </nuxt-link>
        <nuxt-link
          class="nav-item w-1/5 cursor-pointer hover:bg-white hover:text-blue-800 active:bg-white active:text-blue-800 text-center"
          to="/news"
        >
          <li class="h-8 w-8 mt-1">
            <font-awesome-icon :icon="{ prefix: 'fa', iconName: 'newspaper' }" />
          </li>What's New
        </nuxt-link>
        <nuxt-link
          class="nav-item w-1/5 cursor-pointer hover:bg-white hover:text-blue-800 active:bg-white text-center"
          to="/contact"
        >
          <li class="h-8 w-8 mt-1">
            <font-awesome-icon :icon="{ prefix: 'fa', iconName: 'envelope' }" />
          </li>Contact
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
  color: navy;
}
</style>