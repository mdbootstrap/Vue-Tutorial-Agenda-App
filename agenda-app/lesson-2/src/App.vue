<template>
  <mdb-container>
    <mdb-row>
      <mdb-col col="9">Left column</mdb-col>
      <mdb-col col="3">Right column</mdb-col>
    </mdb-row>
  </mdb-container>
</template>

<script>
import { mdbContainer, mdbRow, mdbCol } from "mdbvue";
export default {
  name: "App",
  components: {
    mdbContainer,
    mdbRow,
    mdbCol
  }
};
</script>

<style>
div[class^="col"],
div[class*=" col"] {
  border: 1px dotted black;
}
</style>