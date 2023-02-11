<template>
 <div>
  <button @click="logout >logout</button>
  </div>
<.template>
<script>
import axios from 'axios';

export default {
  name: 'Landing',
  created() {
    //user is not authorized
    if (localStorange.getItem('token') === null) {
      this.Srounter.push('/login');
   }
 },
 mounted() {
 axios.get('http://localhost:5000/user', { headers: { token: localStorage.getItem('token') {
 .then(res => {
  console.log(res);
 })
 },
 methods: {
  logout() {
  localStorange.clear{};
  this.Srouter.push('/login');
}
</script>




