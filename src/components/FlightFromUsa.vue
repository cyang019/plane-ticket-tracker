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
    name: 'flight-from-usa',
    components: {
      FlightList
    },
    data () {
      return {
        origin: '北美',
        airlines: [
          {
            name: '东航',
            flight: 'MU588',
            origCode: 'JFK',
            destCode: 'PVG',
            date: '周三',
            searchLink: 'https://global.ceair.com/shopping?key=JTdCJTIydHJhdmVsVHlwZSUyMiUzQSUyMm9uZXdheSUyMiUyQyUyMnBhc3Nlbmdlck51bSUyMiUzQSUyMjElMkMwJTJDMCUyMiUyQyUyMmRlcENpdHklMjIlM0ElMjJOWUMlMjIlMkMlMjJhcnJDaXR5JTIyJTNBJTIyU0hBJTIyJTJDJTIyZGVwVmFsdWVzJTIyJTNBJTIyRVdSJTJDSkZLJTJDTEdBJTJDU1dGJTIyJTJDJTIyYXJyVmFsdWVzJTIyJTNBJTIyUFZHJTJDU0hBJTIyJTJDJTIyZGVwQ2l0eU5hbWUlMjIlM0ElMjIlRTclQkElQkQlRTclQkElQTYlMjIlMkMlMjJhcnJDaXR5TmFtZSUyMiUzQSUyMiVFNCVCOCU4QSVFNiVCNSVCNyUyMiUyQyUyMmRhdGUlMjIlM0ElMjIyMDIwLTA4LTA1JTIyJTJDJTIyY2FiaW5DbGFzcyUyMiUzQSUyMkFMTCUyMiUyQyUyMnBheVdheSUyMiUzQSUyMm1vbmV5JTIyJTJDJTIyZGVwU2VsZWN0VmFsdWUlMjIlM0ElMjJKRkslMjIlMkMlMjJhcnJTZWxlY3RWYWx1ZSUyMiUzQSUyMlBWRyUyMiUyQyUyMmRlcExhYmVsJTIyJTNBJTIyJUU4JTgyJUFGJUU1JUIwJUJDJUU4JUJGJUFBJUU2JTlDJUJBJUU1JTlDJUJBJTJDJTIwSkZLJTIyJTJDJTIyYXJyTGFiZWwlMjIlM0ElMjIlRTYlQjUlQTYlRTQlQjglOUMlRTUlOUIlQkQlRTklOTklODUlRTYlOUMlQkElRTUlOUMlQkElMkMlMjBQVkclMjIlMkMlMjJpc0FyckNpdHklMjIlM0FmYWxzZSUyQyUyMmlzRGVwQ2l0eSUyMiUzQWZhbHNlJTJDJTIyYXJyQ24lMjIlM0ElMjJDTiUyMiUyQyUyMmRlcENuJTIyJTNBJTIyVVMlMjIlMkMlMjJ0JTIyJTNBMTU5MzIwMzI4ODc3OCU3RA%3D%3DENCODEKEY'
          },
          {
            name: '国航',
            flight: 'CA988',
            origCode: 'LAX',
            destCode: 'TSN',
            date: '周日',
            searchLink: 'https://www.airchina.us/US/CN/info/flight-time/'
          },
          {
            name: '南航',
            flight: 'CZ328',
            origCode: 'LAX',
            destCode: 'CAN',
            date: '周日',
            searchLink: 'https://oversea.csair.com/new/us/zh/flights?m=0&p=200&flex=1&t=LAX-CAN-20200727'
          },
          {
            name: '厦航',
            flight: 'MF830',
            origCode: 'LAX',
            destCode: 'XMN',
            date: '周一',
            searchLink: 'https://www.xiamenair.com/zh-cn/nticket.html?tripType=OW&orgCodeArr%5B0%5D=LAX&dstCodeArr%5B0%5D=XMN&orgDateArr%5B0%5D=2020-08-03&dstDate=&adtNum=2&chdNum=0&isInter=true&JFCabinFirst=false&acntCd='
          },
          {
            name: 'UA (美联航)',
            flight: '[Unknown]',
            origCode: 'SFO',
            destCode: 'PVG',
            date: '?',
            searchLink: 'https://www.united.com/ual/en/CN/flight-search/book-a-flight/results/rev?f=SFO&t=PVG&d=2020-08-05&tt=1&sc=7&px=2&taxng=1&newHP=True&idx=1',
            note: 'Waiting Government Approval'
          },
          {
            name: 'UA (美联航)',
            flight: '[Unknown]',
            origCode: 'EWR',
            destCode: 'PVG',
            date: '?',
            searchLink: 'https://www.united.com/ual/en/CN/flight-search/book-a-flight/results/rev?f=EWR&t=PVG&d=2020-08-05&tt=1&sc=7&px=2&taxng=1&newHP=True&idx=1',
            note: 'Waiting Government Approval'
          },
          {
            name: 'Delta (达美)',
            flight: 'DL287',
            origCode: 'SEA - ICN',
            destCode: 'PVG',
            date: '周四',
            searchLink: 'https://www.delta.com/flight-search/search-results?cacheKeySuffix=7d781b38-f7ca-4a43-8c32-2cb6d082858f'
          },
          {
            name: 'Delta (达美)',
            flight: 'DL282',
            origCode: 'DTW - ICN',
            destCode: 'PVG',
            date: '周五',
            searchLink: 'https://www.delta.com/flight-search/search-results?cacheKeySuffix=06c6aa0b-b2b6-4544-8826-31851b0f23a9'
          }
        ]
      }
    }
}
</script>

<style scoped>

</style>

