<template>
  <div class="my-form">
    <form action="" @submit.prevent>
      <div>
        <label for="">First Name</label>
        <input v-model="student.firstName" type="text" />
        <p>Result is {{ student.firstName }}</p>
      </div>
      <div>
        <label for="">Last Name</label>
        <input v-model="student.lastName" type="text" />
        <p>Result is {{ student.lastName }}</p>
      </div>
      <div>
        <label for="">Age</label>
        <input v-model="student.age" type="number" />
        <p>Result is {{ student.age }}</p>
      </div>
      <div>
        <label for="">Email </label>
        <input v-model="student.email" type="email" />
        <p>Result is {{ student.email }}</p>
      </div>
      <div>
        <h3>favorit Sports</h3>
        <label for="tennis">Tennis</label>
        <input
          v-model="student.sports.tennis"
          type="checkbox"
          name="tennis"
          id="tennis"
        />
        <p>{{ student.sports.tennis }}</p>
        <label for="football">Football</label>
        <input
          v-model="student.sports.football"
          type="checkbox"
          name="football"
          id="football"
        />
        <p>{{ student.sports.football }}</p>
      </div>

      <div class="action" style="width: 100%">
        <input type="submit" style="width: 50%" value="Add" />
      </div>
      <div>
        <ul>
          <li v-for="(st, i) in student" :key="i">
            <p>Name: {{ st.firstName }} {{ st.lastName }}</p>
            <p>Age :{{ st.age }}</p>
            <p>Gender :{{ st.gender }}</p>
            <p>Grade :{{ st.grade }}</p>
            <p>
              favourit Soprts:
              <strong v-for="(sport, i) in st.favouritSoprts" :key="i"
                >{{ sport }}<br />
              </strong>
            </p>
          </li>
        </ul>
      </div>
    </form>
  </div>
</template>

<script>
export default {
  name: "MyForm",
  data() {},
};
</script>

<style>
.my-form {
  form {
    display: flex;
    flex-wrap: wrap;
    div {
      width: 40%;
    }
  }
}
</style>
