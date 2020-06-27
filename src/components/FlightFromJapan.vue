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
      <div class="text-info border-secondary">
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
            searchLink: 'https://www.airchina.us/US/CN/info/flight-time/#'
          },
          {
            name: '厦航',
            flight: 'MF810',
            origCode: 'NRT',
            destCode: 'FOC',
            date: '周五',
            searchLink: 'https://www.xiamenair.com/zh-cn/nticket.html?tripType=OW&orgCodeArr%5B0%5D=NRT&dstCodeArr%5B0%5D=FOC&orgDateArr%5B0%5D=2020-08-07&dstDate=&isInter=true&adtNum=2&chdNum=0&JFCabinFirst=false&acntCd='
          },
          {
            name: '东航',
            flight: 'MU524',
            origCode: 'NRT',
            destCode: 'PVG',
            date: '周五',
            searchLink: 'https://global.ceair.com/shopping?key=JTdCJTIydHJhdmVsVHlwZSUyMiUzQSUyMm9uZXdheSUyMiUyQyUyMnBhc3Nlbmdlck51bSUyMiUzQSUyMjIlMkMwJTJDMCUyMiUyQyUyMmRlcENpdHklMjIlM0ElMjJUWU8lMjIlMkMlMjJhcnJDaXR5JTIyJTNBJTIyU0hBJTIyJTJDJTIyZGVwVmFsdWVzJTIyJTNBJTIySE5EJTJDTlJUJTIyJTJDJTIyYXJyVmFsdWVzJTIyJTNBJTIyUFZHJTJDU0hBJTIyJTJDJTIyZGVwQ2l0eU5hbWUlMjIlM0ElMjIlRTQlQjglOUMlRTQlQkElQUMlMjIlMkMlMjJhcnJDaXR5TmFtZSUyMiUzQSUyMiVFNCVCOCU4QSVFNiVCNSVCNyUyMiUyQyUyMmRlcFNlbGVjdFZhbHVlJTIyJTNBJTIyTlJUJTIyJTJDJTIyYXJyU2VsZWN0VmFsdWUlMjIlM0ElMjJQVkclMjIlMkMlMjJkZXBMYWJlbCUyMiUzQSUyMiVFNiU4OCU5MCVFNyU5NCVCMCVFNSU5QiVCRCVFOSU5OSU4NSVFNiU5QyVCQSVFNSU5QyVCQSUyMiUyQyUyMmFyckxhYmVsJTIyJTNBJTIyJUU2JUI1JUE2JUU0JUI4JTlDJUU1JTlCJUJEJUU5JTk5JTg1JUU2JTlDJUJBJUU1JTlDJUJBJTIyJTJDJTIyaXNBcnJDaXR5JTIyJTNBZmFsc2UlMkMlMjJpc0RlcENpdHklMjIlM0FmYWxzZSUyQyUyMmFyckNuJTIyJTNBJTIyQ04lMjIlMkMlMjJkZXBDbiUyMiUzQSUyMkpQJTIyJTJDJTIyZGF0ZSUyMiUzQSUyMjIwMjAtMDgtMDUlMjIlMkMlMjJjYWJpbkNsYXNzJTIyJTNBJTIyQUxMJTIyJTJDJTIycGF5V2F5JTIyJTNBJTIybW9uZXklMjIlMkMlMjJ0JTIyJTNBMTU5MzI3MjgxMzg4MSU3RA%3D%3DENCODEKEY'
          }
        ]
      }
    }
}
</script>

<style scoped>

</style>
