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
            searchLink: 'http://www.ceair.com/booking/aicn-sha-200807_CNY.html?adt=2&seriesid=1fb20690b81b11ea830ae743cbc28b8d',
          },
          {
            name: '国航',
            flight: 'CA124',
            origCode: 'ICN',
            destCode: 'TAO',
            date: '周五',
            searchLink: 'https://www.airchina.us/US/CN/info/flight-time/#'
          },
          {
            name: '南航',
            flight: 'CZ682',
            origCode: 'ICN',
            destCode: 'SHE',
            date: '周日',
            searchLink: 'https://b2c.csair.com/ita/newIntl/zh/shop/?execution=7f7310649e62f715fbf989b39d53e5e4'
          },
          {
            name: '厦航',
            flight: 'MF872',
            origCode: 'ICN',
            destCode: 'XMN',
            date: '周一',
            searchLink: 'https://www.xiamenair.com/zh-cn/nticket.html?tripType=OW&orgCodeArr%5B0%5D=ICN&dstCodeArr%5B0%5D=XMN&orgDateArr%5B0%5D=2020-08-03&dstDate=&isInter=true&adtNum=2&chdNum=0&JFCabinFirst=false&acntCd='
          },
          {
            name: '大韩',
            flight: 'KE832',
            origCode: 'ICN',
            destCode: 'SHE',
            date: '周五',
            searchLink: 'https://www.koreanair.com/global/en/booking/xiow.html#date-select?paramStrgKey=BOOKING_GATE&isScheduleDriven=false&inflowroute=quickBooking'
          },
          {
            name: '韩亚',
            flight: 'OZ304',
            origCode: 'ICN',
            destCode: 'CGQ',
            date: '周日',
            searchLink: 'https://flyasiana.com/I/CN/CH/RevenueInternationalFareDrivenFlightsSelect.do?E5FdPzdU0umQbR8TUcsLYQ===1596141961',
            note: '谨慎购票， 目的地以后可能会变更'
          },
          {
            name: '济州航空',
            flight: '7C8502',
            origCode: 'ICN',
            destCode: 'WEH',
            date: '周三',
            searchLink: 'https://www.jejuair.net/jejuair/cn/com/jeju/ibe/goAvail.do'
          },
          {
            name: '山东航空',
            flight: 'SC4088',
            origCode: 'ICN',
            destCode: 'TAO',
            date: '周五',
            searchLink: 'http://sc.travelsky.com/scet/queryAvInternational.do',
            note: '行李不能直挂'
          },
          {
            name: '青岛航空',
            flight: 'QW9902',
            origCode: 'ICN',
            destCode: 'TAO',
            date: '周六',
            searchLink: 'http://b2c.qdairlines.com/FlightSearch.do',
            note: '行李不能直挂'
          }
        ]
      }
    }
}
</script>

<style scoped>

</style>