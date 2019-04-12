<template>
  <div>

    <v-subheader id="AcademicTitle" class="title mt-3">Academic Honors Requirements</v-subheader>

    <v-container id="AcaHonors" fluid>
      <v-checkbox v-model="selected" label="`Cumulative GPA of 3.0+`" value="GPA"></v-checkbox>
      <v-checkbox v-model="selected" label="`Geometry`" value="Geometry"></v-checkbox>
      <v-checkbox v-model="selected" label="`Algebra I`" value="AlgI"></v-checkbox>
      <v-checkbox v-model="selected" label="`Algebra II`" value="AlgII"></v-checkbox>
      <v-checkbox v-model="selected" label="`4th Math Credit (Beyond Alg II)`" value="4thMath"></v-checkbox>
      <v-checkbox v-model="selected" label="`Integrated Science`" value="IntegSci"></v-checkbox>
      <v-checkbox v-model="selected" label="`Biology`" value="Bio"></v-checkbox>
      <v-checkbox v-model="selected" label="`3rd Science Credit`" value="3rdSci"></v-checkbox>
      <v-checkbox v-model="selected" label="`4th Science Credit`" value="4thSci"></v-checkbox>
      <v-checkbox v-model="selected" label="`1 AP/IB/Running Start Class Credit`" value="AP1"></v-checkbox>
      <v-checkbox v-model="selected" label="`1 AP/IB/Running Start Class Credit`" value="AP2"></v-checkbox>

      <v-btn onclick="AcademicCheck()">
        <span>Am I Eligible?</span>
      </v-btn>
      <p>{{ selected }}</p>
    </v-container>

  </div>
</template>

<script>

 export default {
    data () {
      return {
        selected: ['Geometry']
      }
    }
  }

</script>
