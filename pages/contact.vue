<template>
  <div class="container mb-3">
    <div>
      <h2 class="subtitle">Contact</h2>
      <div class="content">
        <p
          class="mx-3"
        >Lorem ipsum, dolor sit amet consectetur adipisicing elit. Tenetur repellendus at fuga sapiente odit debitis molestiae et quae recusandae, consectetur quas mollitia quaerat eaque quidem totam odio, dolore praesentium harum.</p>
      </div>
      <img class="mx-auto my-3" src title="Heidi's House Banner" alt="Heidi's House Banner" />
    </div>
  </div>
</template>
<script>
export default {
  head() {
    return {
      title: `About Heidi's House`,
      meta: [
        {
          hid: 'description',
          name: 'description',
          content: `“Heidi’s House” is a pilot program by W.A.G. Healing to explore and
          strengthen the Human and Animal bond toward healing.`
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