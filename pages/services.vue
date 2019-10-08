<template>
  <div class="container mb-3">
    <div>
      <h2 class="title ml-2 md:ml-0">Services</h2>
      <div class="content">
        <h3 class="subtitle"></h3>
        <p class="mx-2">
          Lorem ipsum, dolor sit amet consectetur adipisicing elit. Tenetur repellendus at fuga sapiente
          odit debitis molestiae et quae recusandae, consectetur quas mollitia quaerat eaque quidem totam
          odio, dolore praesentium harum.
        </p>
        <p class="mx-2">
          <img
            class="mx-auto pr-3 float-left h-48 w-48"
            src="../static/me.jpg"
            title="Brian Leabold"
            alt="Brian Leabold"
          />
          Lorem ipsum, dolor sit amet consectetur adipisicing elit. Tenetur repellendus at fuga sapiente
          odit debitis molestiae et quae recusandae, consectetur quas mollitia quaerat eaque quidem totam
          odio, dolore praesentium harum.
        </p>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  head() {
    return {
      title: `Services - Consult Brian`,
      meta: [
        {
          hid: 'description',
          name: 'description',
          content: `From drywall repair and painting, to full bathroom renovations.`
        },
        {
          hid: 'author',
          name: 'author',
          content: 'Brian Leabold'
        }
      ]
    }
  }
}
</script>