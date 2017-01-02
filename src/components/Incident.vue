<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1 {
  color:  #42b983;
}
</style>

<template>
<h1  style="padding:1ex 0">
Service Request
</h1>
<div class="row"  style="padding:2ex 0">
<div class='col-xs-4'>
   Title:
</div>
<div class='col-xs-8'>
<input type="text"></input>
</div>
</div>
<div class="row"  style="padding:2ex 0">
<div class='col-xs-4'>
Description:
</div>

<div class='col-xs-8'>
   <input type="text"></input>
  </div>
</div>
<div style="padding:2ex 0">
  <button class='btn btn-block' style='background-color: #42b983;color:#FFF' @click='submit'>submit</button>
</div>
</template>

<script>
import { submit } from '../Vuex/actions'
export default {
  vuex: {
    actions: {
      submit
    }
  }
}
</script>


