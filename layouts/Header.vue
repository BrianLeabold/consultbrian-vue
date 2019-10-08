<template>
  <header>
    <div class="md:mx-4 flex justify-between text-center rounded-b-lg bg-white text-brand-blue">
      <div
        class="w-1/3 mt-1 py-2 hidden md:block text-xl italic"
      >Professionalism, Pride, Attention to Detail</div>
      <div class="w-full md:w-1/3 m-auto">
        <h1 class="title text-3xl md:text-4xl">Consult Brian</h1>
        <div id="small" class="md:hidden -mt-2 py-2 bg-white text-center mx-auto">
          <p class="italic ml-2">Professionalism, Pride, Attention to Detail</p>
          <div id="socialSmall" class="flex text-center justify-between">
            <div class="w-1/3">
              <a href="https://twitter.com/ConsultBrianSD">
                <font-awesome-icon
                  class="h-8 w-8 text-yellow-900"
                  :icon="{ prefix: 'fab', iconName: 'twitter' }"
                />
              </a>
            </div>
            <div class="w-1/3 text-yellow-900">
              <a href="https://www.instagram.com/consultbriansd/">
                <font-awesome-icon
                  class="h-8 w-8 text-yellow-900"
                  :icon="{ prefix: 'fab', iconName: 'instagram' }"
                />
              </a>
            </div>
            <div class="w-1/3 text-yellow-900">
              <nuxt-link to="/contact">
                <font-awesome-icon
                  class="h-8 w-8 text-yellow-900"
                  :icon="{ prefix: 'fas', iconName: 'envelope' }"
                />
              </nuxt-link>
            </div>
          </div>
        </div>
      </div>
      <div class="w-1/3 mt-1 py-2 hidden md:block">
        <div id="social" class="flex text-center m-auto">
          <a href="https://twitter.com/ConsultBrianSD">
            <font-awesome-icon
              class="h-10 w-10 mt-1 text-yellow-900"
              :icon="{ prefix: 'fab', iconName: 'twitter' }"
            />
          </a>
          <a title="Follow me on Instagram" href="https://www.instagram.com/consultbriansd/">
            <font-awesome-icon
              class="h-10 w-10 mt-1 text-yellow-900"
              :icon="{ prefix: 'fab', iconName: 'instagram' }"
            />
          </a>
          <a href="#contact">
            <font-awesome-icon
              class="h-10 w-10 mt-1 text-yellow-900"
              :icon="{ prefix: 'fas', iconName: 'envelope' }"
            />
          </a>
        </div>
      </div>
    </div>
  </header>
</template>
<script>
export default {
  name: 'Header'
}
</script>