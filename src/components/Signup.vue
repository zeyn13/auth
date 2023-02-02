<template>
  <div>
    NAME: <input type="text" v-model="name" /> <br />
    EMAIL: <input type="text" v-model="email" /> <br />
    PASSWORD: <input type="password" v-model="password" /> <br />
    <button @click="signup">signup</button>
    {{ error }}
  </div>
</template>
<script>
export default {
  name: "Signup",
};
</script>
