<template>
  <div class="col-sm-4 m-0 p-0">
    <div class="d-flex flex-column">
      <flight-list
        :airlines=airlines
        :origin=origin
      ></flight-list>
      <div>
        <p>NRT 三个航站楼， 没有T3摆渡车。KIX没有北美飞机</p>
      </div>
      <div class="text-info">
        <p>衔接航班：</p>
        <div><p>旧金山-东京 UA857</p></div>
        <div><p>纽约-东京 UA79</p></div>
      </div>
    </div>
  </div>  
</template>

<script>
import FlightList from "./FlightList.vue"

export default {
    name: 'flight-from-japan',
    components: {
      FlightList
    },
    data () {
      return {
        origin: '日本东京',
        airlines: [
          {
            name: '国航',
            flight: 'CA930',
            origCode: 'NRT',
            destCode: 'PVG',
            date: '周四',
            searchLink: ''
          },
          {
            name: '厦航',
            flight: 'MF810',
            origCode: 'NRT',
            destCode: 'FOC',
            date: '周五',
            searchLink: ''
          }
        ]
      }
    }
}
</script>

<style scoped>

</style>
