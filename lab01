<script setup>
const accounts = [
  {name : 'salary', amount : 10000},
  {name : 'rent', amount : -2500},
  {name : 'parking fee', amount : 0},
  {name : 'car fuel', amount : -600},
  {name : 'commission', amount : 5500}
]

 function getTotalPrice() {
    return this.accounts.reduce((prev, curr) => {
      return prev + curr.amount;
    }, 0);
 }

</script>

<template>
  <h1>MY ACCOUNT</h1>
  <div v-for ="account in accounts" :key="accounts.amount">
  <p>
      Name : {{ account.name }}<br>
      Amount : <span v-if="account.amount > 0" style="background-color: seagreen;">{{ account.amount }}</span>
               <span v-else-if="account.amount < 0" style="background-color: red;">{{ account.amount }}</span>
               <span v-else></span>
  </p>
      <hr>
  </div>
  <p>{{getTotalPrice()}}</p>

</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
