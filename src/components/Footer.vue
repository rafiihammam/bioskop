<template>
    <p class="copyright">{{ copyright }}</p>
</template>

<script>
export default {
  data () {
    return {
      copyright: 'MLG 2020 Ⓒ chaernh All Rights Reserved'
    }
  },
  year () {
    var d = new Date()
    d.getFullYear()
  }
}

</script>

<style>
    .copyright
    {
        font-style: italic;
        font-size: 10px;
    }
</style>
