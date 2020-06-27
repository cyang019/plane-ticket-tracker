<template>
  <div class="col-sm-4 m-0 p-0">
    <flight-list
      :airlines=airlines
      :origin=origin
    ></flight-list>
  </div>
</template>

<script>
import FlightList from "./FlightList.vue"

export default {
    name: 'flight-from-korea',
    components: {
      FlightList
    },
    data () {
      return {
        origin: '韩国首尔',
        airlines: [
          {
            name: '东航',
            flight: 'MU5042',
            origCode: 'ICN',
            destCode: 'PVG',
            date: '周五',
            searchLink: '',
          },
          {
            name: '国航',
            flight: 'CA124',
            origCode: 'ICN',
            destCode: 'TAO',
            date: '周五',
            searchLink: ''
          },
          {
            name: '南航',
            flight: 'CZ682',
            origCode: 'ICN',
            destCode: 'SHE',
            date: '周日',
            searchLink: ''
          },
          {
            name: '厦航',
            flight: 'MF872',
            origCode: 'ICN',
            destCode: 'XMN',
            date: '周一',
            searchLink: ''
          },
          {
            name: '大韩',
            flight: 'KE832',
            origCode: 'ICN',
            destCode: 'SHE',
            date: '周五',
            searchLink: ''
          },
          {
            name: '韩亚',
            flight: 'OZ304',
            origCode: 'ICN',
            destCode: 'CGQ',
            date: '周日',
            searchLink: '',
            note: '谨慎购票， 目的地以后可能会变更'
          },
          {
            name: '济州航空',
            flight: '7C8502',
            origCode: 'ICN',
            destCode: 'WEH',
            date: '周三',
            searchLink: ''
          },
          {
            name: '山东航空',
            flight: 'SC4088',
            origCode: 'ICN',
            destCode: 'TAO',
            date: '周五',
            searchLink: '',
            note: '行李不能直挂'
          },
          {
            name: '青岛航空',
            flight: 'QW9902',
            origCode: 'ICN',
            destCode: 'TAO',
            date: '周六',
            searchLink: '',
            note: '行李不能直挂'
          }
        ]
      }
    }
}
</script>

<style scoped>

</style>