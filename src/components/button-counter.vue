<template>
<div>
<button v-on:click="count++">You clicked me {{ count }} times.</button>


</div>
  
</template>

<script>
export default {
    data: function () {
    return {
      count: 0
    }
  },
    props: ['title'],
  template: '<h3>{{ title }}</h3>'

}
</script>

<style>