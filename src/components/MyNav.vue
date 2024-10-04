<template>
  <nav class="my-nav">
    <div class="logo">
      <img src="@/assets/nav-logo.png" alt="" />
    </div>
    <div class="links">
      <ul>
        <li v-for="link in links" :key="link">{{ link }}</li>
      </ul>
    </div>
    <div class="btns">
      <button style="">LOGIN</button>
      <BUtton>SIGN Up</BUtton>
    </div>
  </nav>
</template>
<script>
export default {
  data() {
    return {
      logo: "My Logo",
      links: ["Link one", "Link Tow", "Link Three", "Link Four"],
    };
  },
};
</script>
