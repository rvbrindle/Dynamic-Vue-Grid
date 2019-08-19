<template>
  <div id="app">
    <Grid>
      <GridColumn :size='12'>
        <p> 12/12 </p>
      </GridColumn>
    </Grid>
    <Grid>
      <GridColumn :size='6'>
        <p> 6/12 </p>
      </GridColumn>
      <GridColumn :size='6'>
        <p> 6/12 </p>
      </GridColumn>
    </Grid>
     <Grid>
      <GridColumn :size='2'>
        <p> 2/12 </p>
      </GridColumn>
      <GridColumn :size='3'>
        <p> 3/12 </p>
      </GridColumn>
      <GridColumn :size='1'>
        <p> 1/12 </p>
      </GridColumn>
            <GridColumn :size='5'>
        <p> 5/12 </p>
      </GridColumn>
      <GridColumn :size='1'>
        <p> 1/12 </p>
      </GridColumn>
    </Grid>
    <Grid>
      <GridColumn :size='5'>
        <p> 5/12 </p>
      </GridColumn>
      <GridColumn :size='3'>
        <p> 3/12 </p>
      </GridColumn>
      <GridColumn :size='2'>
        <p> 2/12 </p>
      </GridColumn>
      <GridColumn :size='2'>
        <p> 2/12 </p>
      </GridColumn>
    </Grid>
    <Grid>
      <GridColumn :size='4'>
        <p> 4/12 </p>
      </GridColumn>
      <GridColumn :size='4'>
        <p> 4/12 </p>
      </GridColumn>
      <GridColumn :size='4'>
        <p> 4/12 </p>
      </GridColumn>
    </Grid>
    <Grid>
      <GridColumn :size='9'>
        <p> 9/12 </p>
      </GridColumn>
      <GridColumn :size='3'>
        <p> 3/12 </p>
      </GridColumn>
    </Grid>
    <Grid>
      <GridColumn :size='1'>
        <p> 1/12 </p>
      </GridColumn>
      <GridColumn :size='1'>
        <p> 1/12 </p>
      </GridColumn>
      <GridColumn :size='1'>
        <p> 1/12 </p>
      </GridColumn>
      <GridColumn :size='1'>
        <p> 1/12 </p>
      </GridColumn>
      <GridColumn :size='1'>
        <p> 1/12 </p>
      </GridColumn>
      <GridColumn :size='1'>
        <p> 1/12 </p>
      </GridColumn>
      <GridColumn :size='1'>
        <p> 1/12 </p>
      </GridColumn>
      <GridColumn :size='1'>
        <p> 1/12 </p>
      </GridColumn>
      <GridColumn :size='1'>
        <p> 1/12 </p>
      </GridColumn>
      <GridColumn :size='1'>
        <p> 1/12 </p>
      </GridColumn>
      <GridColumn :size='1'>
        <p> 1/12 </p>
      </GridColumn>
      <GridColumn :size='1'>
        <p> 1/12 </p>
      </GridColumn>
    </Grid>
    <Grid>
      <GridColumn :size='7'>
        <p> 7/12 </p>
      </GridColumn>
      <GridColumn :size='5'>
        <p> 5/12 </p>
      </GridColumn>
    </Grid>
  </div>
</template>

<script>
import Grid from "../src/components/Grid"
import GridColumn from "../src/components/GridColumn"
export default {
  name: 'app',
  data() {
    return {

    }
  },
  props: {
    size: {
      type: Number,
      default: 0
    },
  },
  components: {
    Grid,
    GridColumn
  }
}
</script>

<style lang="scss" scoped>
</style>
