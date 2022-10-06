<template>
  <div class="contact-card">
    <div class="contact-card-title">
      {{title}}
    </div>
    <div class="contact-card-image">
      <img :src="image" :alt="title + ' icon'">
    </div>
    <div class="contact-card-url">
      <a :href="url">
        {{url}}
      </a>
    </div>
  </div>
</template>

<script>
let title
let image
let url
export default {
  props: {
    title,
    image,
    url
  },
  name: 'ContactCard'
}
</script>
