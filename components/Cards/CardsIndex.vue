<template>
  <div class="cards_section">
     <Card title="Global Infected" :total_count="globalData.NewConfirmed" :new_count="globalData.TotalConfirmed" desc="Number of active cases"/>
     <Card title="Global Recovered" :total_count="globalData.NewRecovered" :new_count="globalData.TotalRecovered" desc="Number of recoveries"/>
     <Card title="Global Deaths" :total_count="globalData.NewDeaths" :new_count="globalData.TotalDeaths" desc="Number of deaths"/>
  </div>
</template>

<script>
import Card from './Card';
export default {
 props:['globalData'],
 components:{
     Card
 }
}
</script>

<style>

</style>