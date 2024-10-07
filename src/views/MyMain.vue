<template>
  <div class="my-main">
    <h1>This is my main page</h1>
    <MyForm />
  </div>
</template>

<script>
import MyForm from "@/components/MyFrom.vue";

export default {
  name: "MyMain",
  components: {
    MyForm,
  },
  data() {},
};
</script>

<style>
.my-nav {
  display: flex;
  justify-content: space-between;
  align-items: center;
  background: gray;
  box-shadow: 0px 0px 0px 0px black;
}
ul {
  display: flex;
  justify-content: space-between;
  gap: 20px;
  list-style-type: none;
}

img {
  width: 15%;
}

button {
  background-color: rgb(42, 112, 112);
  color: white;
  padding: 5px 10px;
}
</style>
