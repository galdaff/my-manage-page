<template>
  <div class="container">
    <div class="col">
      <div class="col-1">
        <div class="row">
          <div class="col-md-1">
            <div class="header"></div>
            <div class="body">information</div>
            <div class="footer">footer</div>
          </div>
        </div>
        <div class="row">
          <div class="col-md-1">
            <h1 class="h1">User 1</h1>
            <br />
            <h2 class="h2">User 2</h2>
          </div>
        </div>
        <div class="row">
          <div class="col-md-1">
            <h1 class="h1">User 1</h1>
            <br />
            <h2 class="h2">User 2</h2>
          </div>
        </div>
        <div class="row">
          <div class="col-md-1">
            <h1 class="h1">User 1</h1>
            <br />
            <h2 class="h2">User 2</h2>
          </div>
        </div>
      </div>
      <div class="col-1">
        <div class="row">
          <div class="col-md-1">
            <h1 class="h1">User 1</h1>
            <br />
            <h2 class="h2">User 2</h2>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import { Component, Prop, Vue } from 'vue-property-decorator'

@Component
export default class HelloWorld extends Vue {
  @Prop() private msg!: string;
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.container {
  width: 1695px;
  min-height: 700px;
  overflow: hidden;
  border-radius: 3px;
  border-width: 1px;
  border-style: solid;
  display: flex;
}
.col {
  display: table;
  table-layout: fixed;
  border-spacing: 1rem;
}
.col-1 {
  display: table-row;
}
.row {
  width: 400px;
  height: 190px;
  border-radius: 3px;
  border-width: 1px;
  border-style: solid;
  display: table-cell;
}
.col-md-1 {
  display: inline-block;
  min-height: 200px;
  overflow: hidden;
}
.header {
  width: 400px;
  height: 90px;
  border-radius: 3px;
  border-width: 1px;
  border-style: solid;
  background-color: aqua;
}
.body {
  height: 400px;
  border-radius: 3px;
  border-width: 1px;
  border-style: solid;
}
.footer {
  height: 97px;
  border-radius: 3px;
  border-width: 1px;
  border-style: solid;
}
.h1 {
  border-radius: 3px;
  border-width: 1px;
  border-style: solid;
}
.h2 {
  border-radius: 3px;
  border-width: 1px;
  border-style: solid;
}
</style>
