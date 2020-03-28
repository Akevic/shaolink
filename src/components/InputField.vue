<template>
  <div class="input-field">
    <input type="text" class="input-url" placeholder="Shorten a link here..." v-model="URL">
    <button class="url-button" type="button">Shorten It!</button>
  </div>
</template>

<script>
export default {
  name: 'InputField',
  data () {
    return {
      URL: ''
    }
  }
}
</script>

<style lang="scss" scoped>
  .input-field {
    display: flex;
    flex-direction: column;

    background-image: url('../assets/bg-shorten-mobile.svg');
    background-size: 1000%;
    padding: 1.5rem;
    margin-top: 4rem;
    border-radius: 15px;

    .input-url {
      width: 80%;
      margin: 0 auto;
      margin-bottom: 1rem;
      outline: none;
    }

    .url-button {
      width: 86.5%;
      margin: 0 auto;
      border-radius: 10px;
      border: 1px solid #F69487;
      background-color: #F69487;
      padding: .3rem 1rem;
      font-size: 1rem;
      color: #fff;
      cursor: pointer;
    }

    &.desktop {
      display: none;
      @media (min-width: 992px) {
        display: flex;
        flex-direction: row;

        width: 60%;
        margin: 0 auto;
        padding: 2rem;

        .input-url {
          margin-bottom: 0;
          margin-right: 2rem;
          padding: .7rem;
        }

        .url-button {
          width: 20%;
          border-radius: 10px;
        }
      }
    }

  }
</style>
