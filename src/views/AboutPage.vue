<template>
  <div class="about">
    <h2>This is the about page</h2>
    <MyCont :students="students" />
  </div>
</template>

<script>
import MyCont from "@/components/MyContent.vue";

export default {
  components: {
    MyCont,
  },
  data() {
    return {
      students: ["Randa", "Asia", "Rawan"],
    };
  },
};
</script>
