<template>
  <div class="home">
    <div id="read"></div>
    <span class="icon-bookmark"></span>
  </div>
</template>

<script>
// @ is an alias to /src
import Epub from 'epubjs'
global.ePub = Epub

export default {
  name: 'home',
  mounted () {
    this.book = new Epub('/2017_Book_InterdisciplinaryPerspectivesO.epub')
    this.book.renderTo('read', {
      width: window.innerWidth,
      height: window.innerHeight
    }).display()
  }
}
</script>
