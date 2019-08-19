<template>
  <header>
      <p>{{propsdata}}</p>
      <button v-on:click="sendEvent">Send</button>
  </header>
</template>

<script>
export default {
    props: ['propsdata'],
    methods:{
        sendEvent: function(){
            this.$emit('renew');
        }
    }
}
    
</script>

<style>

</style>