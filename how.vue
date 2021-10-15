<template>
  <div class="p-4 grid row-4 gap-4">
    <div v-for="array in array" :key="array.id" class="p-2 border-2 rounded-lg">
      <h1>{{ array.name }}</h1>
      <h1>age: {{ array.age }}</h1>
    </div>
  </div>
</template>
<script>
export default {
  name: "How",
  data: () => ({
    array: [
      {
        name: "Adam",
        age: 19,
      },
      {
        name: "Amar",
        age: 22,
      },
      {
        name: "Asma",
        age: 16,
      },
      {
        name: "Nadia",
        age: 14,
      },
      {
        name: "Oussama",
        age: 18,
      },
      {
        name: "Lina",
        age: 26,
      },
    ],
  }),
};
</script>
