<template>
  <div class="contact-card">
    <div class="contact-card-image">
      <!-- FIXME duplicated code -->
      <a :href="'mailto:'+url" v-if="kind==='email'">
        <slot></slot>
      </a>
      <a :href="'tel:'+url" v-else-if="kind==='tel'">
        <slot></slot>
      </a>
      <a :href="url" target="_blank" v-else>
        <slot></slot>
      </a>
    </div>
    <div class="contact-card-title">
      {{title}}
    </div>
    <div class="contact-card-url">
      <a :href="'mailto:'+url" v-if="kind==='email'">
        {{url}}
      </a>
      <a :href="'tel:'+url" v-else-if="kind==='tel'">
        {{url}}
      </a>
      <a :href="url" target="_blank" v-else>
        {{url}}
      </a>
    </div>
  </div>
</template>

<script>
let title
let image
let url
let kind
export default {
  props: {
    title,
    image,
    url,
    kind
  },
  name: 'ContactCard'
}
</script>
