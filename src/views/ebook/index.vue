<template>
  <div class="ebook">
    <ebook-title></ebook-title>
    <ebook-reader></ebook-reader>
    <ebook-menu></ebook-menu>
  </div>
</template>

<script>
import EbookTitle from '../../components/ebook/EbookTitle'
import EbookReader from '../../components/ebook/EbookReader'
import EbookMenu from '../../components/ebook/EbookMenu'

export default {
  components: {
    EbookTitle,
    EbookReader,
    EbookMenu
  }
}
</script>

<style lang='scss' scoped>
@import '../../assets/styles/global';

.ebook {
  font-size: px2rem(20);
}
</style>
