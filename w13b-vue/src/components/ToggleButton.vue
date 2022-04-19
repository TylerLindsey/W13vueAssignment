<template>
  <div>
    <button>Toggle</button>
    <Toggle v-model="value" :options="options"/>
  </div>
</template>

<script>
  export default {
    name: 'ToggleButton',
    data(){
      return{
        value: 'grid'
      }
    }
  }
</script>

<style scoped>
button{
  background-color: rgb(224, 206, 206);
}
</style>