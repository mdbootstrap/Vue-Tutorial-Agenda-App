<template>
  <mdb-container>
    <mdb-row>
      <mdb-col col="9">
        <Event time="10:00" title="Breakfast with Simon" location="Lounge Caffe" description="Discuss Q3 targets"/>
        <Event time="10:30" title="Daily Standup Meeting (recurring)" location="Warsaw Spire Office"/>
      </mdb-col>
      <mdb-col col="3"></mdb-col>
    </mdb-row>
  </mdb-container>
</template>

<script>
import { mdbContainer, mdbRow, mdbCol } from "mdbvue";
import Event from "@/components/Event";
export default {
  name: "App",
  components: {
    mdbContainer,
    mdbRow,
    mdbCol,
    Event
  }
};
</script>

<style>
div[class^="col"],
div[class*=" col"] {
  border: 1px dotted black;
}
</style>