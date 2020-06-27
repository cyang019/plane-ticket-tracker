<template>
  <div class="d-flex card card-body m-1 p-1 border border-primary">
    <div class="d-flex flex-row">
      <div v-if="['国航', '南航', '厦航', '东航', '山东航空', '青岛航空'].includes(name)" class="card-text text-secondary">
        <strong>{{name}}</strong>
      </div>
      <div v-else class="card-text text-primary">
        <strong>{{name}}</strong>
      </div>
      <a :href="searchLink" target="_blank"
        @click="incrementCount"
      >
        <span class="card-text">{{flight}} </span>
        <span class="card-text">{{origCode}} - {{destCode}}</span>
        <span class="card-text"> {{date}}</span>
      </a>
    </div>
    <p class="card-text text-info">{{note}}</p>
  </div>
</template>

<script>
export default {
    name: 'flight-list',
    props: [
      'name', 'flight',
      'origCode', 'destCode', 'date',
      'searchLink', 'note'
    ],
    data () {
      return {
        count: 0
      }
    },
    methods: {
      init () {
        this.count = 0
      },
      incrementCount () {
        ++this.count
      }
    },
    mounted: function() {
      this.init()
    }
}
</script>

<style scoped>

</style>