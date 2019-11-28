<template>
  <section>
    <h1 v-if="$device.isDesktop">
      Desktop
    </h1>
    <div v-if="$device.isMobile">
      Mobile
    </div>
  </section>
</template>

<script>

export default {
  layout: ctx => ctx.isMobile ? 'mobile' : 'main'

}
</script>

<style>
div {
  color: #fff;
}
</style>
