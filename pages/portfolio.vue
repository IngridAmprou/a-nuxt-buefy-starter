<template>
  <section>
    <div class="hero-body">
      <div class="container has-text-centered">
        <h1 class="title pb-4">
          Your NuxtJS projects
        </h1>
        <h2 class="subtitle">
          Show your work
        </h2>
      </div>
    </div>     
  </section>
</template>

<script>
export default {
  head: {
    title: 'Portfolio',
    meta: [
      {
        hid: 'description',
        name: 'description',
        content: 'description'
      }
    ],
  },
  transition: 'bounce',  
}
</script>