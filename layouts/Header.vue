<template>
  <header>
    <div class="md:mx-4 flex justify-between text-center rounded-b-lg bg-white text-brand-blue">
      <div
        class="w-1/3 py-2 hidden md:block text-xl italic"
      >Professionalism, Pride, Attention to Detail</div>
      <div class="w-full md:w-1/3 m-auto">
        <h1 class="title text-3xl md:text-4xl">Consult Brian</h1>
        <div id="small" class="md:hidden -mt-2 py-2 bg-white text-center mx-auto">
          <p class="italic ml-2">Professionalism, Pride, Attention to Detail</p>
          <div id="socialSmall" class="flex text-center justify-between">
            <div class="w-1/3 text-yellow-900">
              <a href="https://twitter.com/ConsultBrianSD">
                <i class="fab fa-2x fa-twitter"></i>
              </a>
            </div>
            <div class="w-1/3 text-yellow-900">
              <a href="https://www.instagram.com/consultbriansd/">
                <i class="fab fa-2x fa-instagram"></i>
              </a>
            </div>
            <div class="w-1/3 text-yellow-900">
              <a href="#contact">
                <i class="fas fa-2x fa-envelope"></i>
              </a>
            </div>
          </div>
        </div>
      </div>
      <div class="w-1/3 py-2 hidden md:block">
        <div id="social" class="flex text-center m-auto">
          <a href="https://twitter.com/ConsultBrianSD">
            <i class="mr-12 fab fa-3x fa-twitter text-yellow-900"></i>
          </a>
          <a href="https://www.instagram.com/consultbriansd/">
            <i class="mr-12 fab fa-3x fa-instagram text-yellow-900"></i>
          </a>
          <a href="#contact">
            <i class="fas fa-3x fa-envelope text-yellow-900"></i>
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