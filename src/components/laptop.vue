<template>
  <div class="user">
     <a href="home">Home</a>
    <a href="home">login / sign up</a>
    <a href="home">About us</a>
    <a href="home">facebook</a>
  </div>
</template>
<script>
export default {
  name: "laptop",
};
</script>

<style >
.user {
  padding: 30px;
  text-decoration: none;
  text-align: center;
  text-justify: center;
}
.user a {
  color: #f2f2f2;
  margin: 17px;
  padding: 20px;
  text-decoration: none;
  background-color: #333;
  font-size: 22px;
  border-radius: 0 10px;
}
.user a:hover{
    box-shadow: 4px 10px #3a003a;
}
</style>