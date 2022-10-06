<template>
  <div class="section contact-section">
    <div class="container mx-auto">
      <div class="section-title-container">
        <div class="larger-title">Kontakt</div>
      </div>
      <div class="section-content-container contact-card-container">
        <ContactCard title="Github" url="https://github.com/Gumkle" image="github.svg" />
        <ContactCard title="E-mail" url="kontakt.dawid.dziedzic@gmail.com" image="email.svg" />
        <ContactCard title="LinkedIn" url="https://www.linkedin.com/in/dawid-dziedzic-8b0a61141/" image="linkedin.svg" />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'ContactSection'
}
</script>
