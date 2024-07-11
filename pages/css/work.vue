<template>
  <div>
    <!-- ここの間にHTMLを書いてください -->
    <div class="sample">
      <h2>Sample Color App</h2>
      <input type="color" id="color" v-model="color" />
    </div>
  </div>
</template>

<style>
/** ここの間にCSSを書いてください **/
.sample h2{
  color: v-bind(color);
}
</style>

<script>
  import Vue from "vue";
  export default{
    data() {
      return{
        color: "#FF0000"
      };
    }
  }
</script>
