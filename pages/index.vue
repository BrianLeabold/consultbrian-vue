<template>
  <div class="container md:mb-3 mb-24">
    <div>
      <h2 class="subtitle">A Little About Me</h2>
      <div class="content">
        <h3>Grandson of a carpenter Son of a remodeler</h3>
        <p class="mx-2">
          <img
            class="mx-auto my-3 float-right"
            src="../static/me.jpg"
            title="Brian Leabold"
            alt="Brian Leabold"
          />
          I started swinging a hammer the summer I turned 12. Nailing down plywood sub-floor by hand,
          side by side with my grand-dad and my father, is a fond memory that has fueled my love of
          construction all my life. Through out high school I worked for my dad on the weekends and
          over summer vacations. He taught me about dealing with other trades, suppliers and our own customers.
        </p>
        <p>
          Then in September of my senior year of high school, I decided to join the Navy. Building on what
          I learned working for my father, I learned more about people and their plethora of personalities.
          I was able to see places and things that has fueled my ability to envision the big picture, yet
          focus on important details that make my projects feel complete.
        </p>
        <p>
          <nuxt-link to="/contact">Schedule your free consultation today</nuxt-link>
        </p>
        <h3>Providing an array of services for my customers</h3>
        <p>
          From advice and assistance on small projects; to design, layout`, and contractor liaison. Do you have
          an idea or a concept you like, but you don't know if it's possible? I can help with that. Have a DIY
          project you want to tackle? I will provide a material list for you. Need a hand with something? I have two.
        </p>
        <p>
          It's never easy managing large construction/remodeling projects. By setting up timelines and goals with your
          contractors and only billing you my actual time, you can save money over using a GC.
        </p>
        <p>
          <nuxt-link to="/services">More about the services I provide</nuxt-link>
        </p>
      </div>
    </div>
  </div>
</template>

<script>
import Logo from '~/components/Logo.vue'

export default {
  components: {
    Logo
  }
}
</script>

<style>
/* Sample `apply` at-rules with Tailwind CSS */
</style>
