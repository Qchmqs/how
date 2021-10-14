<template>
    <div class="p-4 grid row-4 gap-4">
      <div v-for="user in users" :key="array.id" class="p-2 border-2 rounded-lg">
        <h1>{{user.name}}</h1>
        <h1>age : {{user.age}}</h1>
      </div>
    </div>
</template>
<script>
import _ from 'lodash'
export default {
  name: "How",
  components: {},
  data() {
    return {
    };
  },
  methods: {},
  computed:{
    users() {
        const arr = [
        {
          name : "Adam",
          age : 19,
        },
        {
          name : "Amar",
          age : 22
        },
        {
          name : "Asma",
          age : 16
        },
        {
          name : "Nadia",
          age : 14,
        },
        {
          name : "Oussama",
          age : 18
        },
        {
          name : "Lina",
          age : 26
        },
      ]
      return _.sortBy(users, ['age'])
    }
  },
};
</script>
