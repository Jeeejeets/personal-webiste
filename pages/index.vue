<template>
  <div class="root">
    <UpperNavbar/>
    <TitleSection/>
    <WhoamiSection/>
    <ContactSection />
  </div>
</template>

<script>
export default {
  name: 'IndexPage',
  head () {
    return {
      title: 'Dawid Dziedzic - personal page'
    }
  }
}
</script>
