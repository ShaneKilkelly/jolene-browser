<template>
  <div id="page" class="container">
    <div class="columns is-mobile">
      <div id="page-wrapper" class="column is-8 is-offset-2 content">

        <iframe frameborder="0"
                name="renderedPage"
                :srcdoc="currentTabSrc"
                sandbox="allow-same-origin allow-scripts">
        </iframe>

      </div>
    </div>
  </div>
</template>

<style scoped>
 page-wrapper {
   height: 100%;
   overflow: scroll;
 }
 iframe {
   width: 100%;
   height: 100%;
   min-height: 600px;
 }
</style>

<script>
 import PageDisplay from './PageDisplay.js';
 export default PageDisplay;
</script>
