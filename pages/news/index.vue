<template>
  <div class="container mb-3">
    <section id="whatsnew-page" class="text-center md:text-left md:ml-8">
      <h2 class="title">What's New</h2>
      <p>A wide variety of projects I am involved in, from remodeling to reducing our impact on our world.</p>
      <div class="content flex flex-wrap flex-column justify-around">
        <PostPreview
          v-for="post in posts"
          :key="post.id"
          :title="post.title"
          :excerpt="post.excerpt"
          :thumbnailImage="post.thumbnailImage"
          :id="post.id"
          :postDate="post.postDate"
        />
      </div>
    </section>
  </div>
</template>
<script>
import PostPreview from '@/components/Blog/PostPreview'
export default {
  components: {
    PostPreview
  },
  head() {
    return {
      title: `What's New`,
      meta: [
        {
          hid: 'description',
          name: 'description',
          content: `A wide variety of projects I am involved in, from remodeling to reducing our impact on our world.`
        },
        {
          hid: 'author',
          name: 'author',
          content: 'Brian Leabold'
        }
      ]
    }
  },
  // data() {
  //   return {
  //     posts: [
  //       {
  //         title: `Recycle, Reduce, Reuse - Part 2`,
  //         previewText: `Are you looking for a way to lower your impact on our environment? Use the power of the sun to generate your hot water.`,
  //         thumbnailUrl: `https://consultbrian.com/assets/images/solarshower/solarshower-3.jpg`,
  //         id: `recycle-reduce-reuse-part-2`,
  //         postDate: `April 12th, 2019`
  //       },
  //       {
  //         title: `Recycle, Reduce, Reuse - Part 1`,
  //         previewText: `This simple project will do just that.`,
  //         thumbnailUrl: `https://consultbrian.com/assets/images/compost_toilet-9.jpg`,
  //         id: `recycle-reduce-reuse-part-1`,
  //         postDate: `March 18th, 2019`
  //       },
  //       {
  //         title: `San Diego Waives Permit Fees`,
  //         previewText: `The San Diego County Board of Supervisors voted unanimously in an attempt to fight the affordable housing crisis.`,
  //         thumbnailUrl: `https://consultbrian.com/assets/images/granny-flats.jpg`,
  //         id: `san-diego-county-waives-permit-fees`,
  //         postDate: `January 18th, 2019`
  //       },
  //       {
  //         title: `A New Beginning`,
  //         previewText: `This will be awesome`,
  //         thumbnailUrl: ``,
  //         id: `a-new-beginning`,
  //         postDate: `12/1/2018`
  //       }
  //     ]
  //   }
  // }

  asyncData(context) {
    // Check if we are in the editor mode
    let version =
      context.query._storyblok || context.isDev ? 'draft' : 'published'

    // Load the JSON from the API
    return context.app.$storyapi
      .get('cdn/stories', {
        version: 'draft',
        starts_with: 'news/'
      })
      .then(res => {
        console.log(res.data)
        return {
          posts: res.data.stories.map(bp => {
            return {
              id: bp.slug,
              thumbnailImage: bp.content.thumbnailImage,
              title: bp.content.title,
              postDate: bp.content.postDate,
              excerpt: bp.content.excerpt
            }
          })
        }
      })
      .catch(res => {
        context.error({
          statusCode: res.response.status,
          message: res.response.data
        })
      })
  }
}
</script>