<template>
<div>
  <main class="hero mobile">
    <img :src="require('@/assets/hero_image.svg')" alt="Hero image" class="hero-image">
    <h1 class="hero-title">More than just shorter links</h1>
    <p class="hero-text">Build your brand's recognition and get detailed insights on how your links are performing</p>
    <button class="hero-button" type="button">Get Started</button>
    <InputField />
  </main>
  <main class="hero desktop">
    <div class="col-left">
    <h1 class="hero-title">More than just shorter links</h1>
    <p class="hero-text">Build your brand's recognition and get detailed <br> insights on how your links are performing</p>
    <button class="hero-button" type="button">Get Started</button>
    </div>
    <div class="col-right">
    <img :src="require('@/assets/hero_image.svg')" alt="Hero image" class="hero-image">
    </div>
  </main>
  <InputField class="desktop" />
</div>
</template>

<script>
import InputField from '@/components/InputField.vue'

export default {
  name: 'Hero',
  components: {
    InputField
  }
}
</script>
