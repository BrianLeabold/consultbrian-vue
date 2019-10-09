<template>
  <div class="mb-3 max-w-xs md:mx-4 md:w-1/4 align-middle text-center">
    <nuxt-link :to="`/news/${id}`">
      <article class="post-preview border-b border-blue-900 shadow-md overflow-hidden">
        <div
          :style="{backgroundImage:  'url(' + thumbnailImage + ')'}"
          class="thumbnail-preview h-48 full-width bg-cover mt-4 left-align"
        ></div>
        <div class="post-preview-content m-1 items-center">
          <h3 class="subtitle">{{title}}</h3>
          <small class="italic">{{postDate}}</small>
          <p class="truncate">{{excerpt}}</p>
        </div>
      </article>
    </nuxt-link>
    <hr />
  </div>
</template>
<script>
export default {
  props: {
    title: {
      type: String,
      required: true
    },
    excerpt: {
      type: String,
      required: true
    },
    thumbnailImage: {
      type: String,
      required: true
    },
    id: {
      type: String,
      required: true
    },
    postDate: {
      type: String,
      required: true
    }
  }
}
</script>