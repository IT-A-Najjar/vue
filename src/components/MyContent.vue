<template>
  <div class="mycontent">
    <ul>
      <li v-for="(student, i) in students" :key="i">
        {{ student }}
      </li>
    </ul>
    <button @click="deleteSt">Change Ref</button>
    <p>active is: {{ myActive }}</p>
    <button @click="($event) => $emit('updateActive', false)">
      Change Prem
    </button>
  </div>
</template>

<script>
export default {
  props: {
    students: {
      type: Array,
      required: true,
    },
    isActive: {
      type: Boolean,
    },
  },
  emits: ["updateActive"], // تأكد من كتابة "updateActive" بشكل صحيح
  data() {
    return {
      myStudents: this.students,
      myActive: this.isActive,
    };
  },
  methods: {
    deleteSt() {
      this.myStudents.shift();
    },
    changeActive() {
      this.$emit("updateActive", false);
    },
  },
};
</script>

<style scoped>
ul {
  list-style: none;
  display: flex;
  justify-content: center;
  gap: 20px;
}
</style>
