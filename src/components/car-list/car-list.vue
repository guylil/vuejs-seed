<template lang="html">


  <section class="car-list">
    <h3>Cars List</h3>
    <div class="row">
      <div class="col-xs-18 col-sm-4" v-for="car of cars">
          <car-preview class="card"  v-bind:car="car"></car-preview>
      </div>

    </div>
    
  </section>
</template>

<script lang="js">
  import CarPreview from '../car-preview/car-preview';
  export default  {
    name: 'car-list',
    props: [],
    mounted() {

    },
    data() {
      return {
        cars: [{name: 'Ugi', power: 3}, {name: 'Shraga', power: 4}]
      }
    },
    methods: {

    },
    computed: {

    },
    components: {
      CarPreview
    }
}
</script>

<style scoped lang="scss">
  .car-list {

    

  }
</style>
