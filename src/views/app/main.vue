<style src='style.scss' lang='scss'></style>
<script src='script.js'></script>
<template>
  <div class='app'>
    <div class='_layer -inner -wrap _wrap'>
      <v-compare></v-compare>
      <page></page>
      <pagination></pagination>
    </div>
    <transition name='fade'>
      <div class='_layer -wrap _wrap' v-if='modal === "compare"'>
        <modal>
          <compare-modal></compare-modal>
        </modal>
      </div>
    </transition>
    <!-- <v-appbar></v-appbar> -->
  </div>
</template>
