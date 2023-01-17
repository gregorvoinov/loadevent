<template>
  <div>
    <img
      src="https://nuxt.studio/landing.png"
      @load="onLoad"
      style="width: 50%"
    />
    <img
        src="/images/img1.jpg"
        @load="onload"
        @error="onLoadLocal"
        style="width: 50%"
    />
  </div>
</template>

<script setup>
  const onLoad = (e) => {
    console.log('looooaded', e);
  }
  const onLoadLocal = (e) => {
    console.log('looooaded local', e);
  }
</script>
