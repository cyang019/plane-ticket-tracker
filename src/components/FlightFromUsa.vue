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
            origCode: '纽约肯尼迪JFK',
            destCode: '上海浦东PVG',
            date: '周三',
            searchLink: 'https://global.ceair.com/shopping?key=JTdCJTIydHJhdmVsVHlwZSUyMiUzQSUyMm9uZXdheSUyMiUyQyUyMnBhc3Nlbmdlck51bSUyMiUzQSUyMjElMkMwJTJDMCUyMiUyQyUyMmRlcENpdHklMjIlM0ElMjJOWUMlMjIlMkMlMjJhcnJDaXR5JTIyJTNBJTIyU0hBJTIyJTJDJTIyZGVwVmFsdWVzJTIyJTNBJTIyRVdSJTJDSkZLJTJDTEdBJTJDU1dGJTIyJTJDJTIyYXJyVmFsdWVzJTIyJTNBJTIyUFZHJTJDU0hBJTIyJTJDJTIyZGVwQ2l0eU5hbWUlMjIlM0ElMjIlRTclQkElQkQlRTclQkElQTYlMjIlMkMlMjJhcnJDaXR5TmFtZSUyMiUzQSUyMiVFNCVCOCU4QSVFNiVCNSVCNyUyMiUyQyUyMmRhdGUlMjIlM0ElMjIyMDIwLTA4LTA1JTIyJTJDJTIyY2FiaW5DbGFzcyUyMiUzQSUyMkFMTCUyMiUyQyUyMnBheVdheSUyMiUzQSUyMm1vbmV5JTIyJTJDJTIyZGVwU2VsZWN0VmFsdWUlMjIlM0ElMjJKRkslMjIlMkMlMjJhcnJTZWxlY3RWYWx1ZSUyMiUzQSUyMlBWRyUyMiUyQyUyMmRlcExhYmVsJTIyJTNBJTIyJUU4JTgyJUFGJUU1JUIwJUJDJUU4JUJGJUFBJUU2JTlDJUJBJUU1JTlDJUJBJTJDJTIwSkZLJTIyJTJDJTIyYXJyTGFiZWwlMjIlM0ElMjIlRTYlQjUlQTYlRTQlQjglOUMlRTUlOUIlQkQlRTklOTklODUlRTYlOUMlQkElRTUlOUMlQkElMkMlMjBQVkclMjIlMkMlMjJpc0FyckNpdHklMjIlM0FmYWxzZSUyQyUyMmlzRGVwQ2l0eSUyMiUzQWZhbHNlJTJDJTIyYXJyQ24lMjIlM0ElMjJDTiUyMiUyQyUyMmRlcENuJTIyJTNBJTIyVVMlMjIlMkMlMjJ0JTIyJTNBMTU5MzIwMzI4ODc3OCU3RA%3D%3DENCODEKEY'
          },
          {
            name: '国航',
            flight: 'CA988',
            origCode: '洛杉矶LAX',
            destCode: '天津滨海TSN',
            date: '周日',
            searchLink: 'https://www.airchina.us/US/CN/info/flight-time/'
          },
          {
            name: '南航',
            flight: 'CZ328',
            origCode: '洛杉矶LAX',
            destCode: '广州白云CAN',
            date: '周日',
            searchLink: 'https://oversea.csair.com/new/us/zh/flights?m=0&p=200&flex=1&t=LAX-CAN-20200727'
          },
          {
            name: '厦航',
            flight: 'MF830',
            origCode: '洛杉矶LAX',
            destCode: '厦门高崎XMN',
            date: '周一',
            searchLink: 'https://www.xiamenair.com/zh-cn/nticket.html?tripType=OW&orgCodeArr%5B0%5D=LAX&dstCodeArr%5B0%5D=XMN&orgDateArr%5B0%5D=2020-08-03&dstDate=&adtNum=2&chdNum=0&isInter=true&JFCabinFirst=false&acntCd='
          },
          {
            name: 'UA (美联航)',
            flight: 'UA857',
            origCode: '旧金山SFO',
            destCode: '上海浦东PVG',
            date: '周三，周六',
            searchLink: 'https://www.united.com/zh-hans/cn',
            note: ''
          },
          {
            name: 'Delta (达美)',
            flight: 'DL287',
            origCode: '西雅图SEA - 首尔ICN',
            destCode: '上海浦东PVG',
            date: '周四',
            searchLink: 'https://zh.delta.com/cn/zh'
          },
          {
            name: 'Delta (达美)',
            flight: 'DL282',
            origCode: '底特律DTW - 首尔ICN',
            destCode: '上海浦东PVG',
            date: '周五',
            searchLink: 'https://zh.delta.com/cn/zh'
          }
        ]
      }
    }
}
</script>

<style scoped>

</style>

