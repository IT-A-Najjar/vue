<template>
  <div class="my-main">
    <h1>this is my main page</h1>
    
    <!-- <MyFrom /> -->
  
    </div>
</template>
<script>
import MyFrom from "@/components/MyFrom.vue";
//import MyComponent from "@/components/MyComponent.vue";
//import MyComponentTow from "@/components/MyComponent.vue";
//import MyCont from "@/components/MyContent.vue";
//import LifeCycle from "@/components/LifeCycle.vue";

export default {
  name: "MyMain",
  components: {
    //MyFrom,
  },
  data() {
    
      
    }
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
