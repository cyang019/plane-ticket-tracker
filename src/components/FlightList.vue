<template>
  <div class="card border-primary">
    <div class="card-header bg-dark text-light">
      <h3>{{origin}}</h3>
    </div>
    <div class="card-body">
      <ul class="list-group list-group-flush">
        <li v-for="(airline, index) in airlines" :key=index
          class="list-group-item m-0 p-0"
        >
          <airline-item
            :name=airline.name
            :flight=airline.flight
            :origCode=airline.origCode
            :destCode=airline.destCode
            :date=airline.date
            :searchLink=airline.searchLink
            :note=airline.note
          ></airline-item>
        </li>
      </ul>
    </div>
  </div>
    
</template>

<script>
import AirlineItem from "./AirlineItem.vue"

export default {
    name: 'flight-list',
    props: ['airlines', 'origin'],
    components: {
      AirlineItem
    }
}
</script>

<style scoped>

</style>
