<template>
  <section>
    <div>
      <div id="SOHUCS" :sid="sendEssayId"></div>
    </div>
  </section>
</template>
<script>
export default {
  data() {
    return {
    }
  },
  props: ['sendEssayId'],
  mounted() {
    this.$nextTick(() => {
      setTimeout(() => {
        window.changyan.api.config({
          appid: 'cyu8TykID',
          conf: 'prod_f93bf75ab6b5618003d9a02c4e56cc6d'
        })
      }, 0);
    })
  }
}
</script>
<style lang="less">
 /deep/ .module-cmt-list,.section-list-w {
   display: none;
 }
</style>
