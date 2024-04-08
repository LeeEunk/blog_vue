<template>
  <div class="container mt-4">
    <h5 @click="$router.push('/detail/0')">{{ data[0].title }}</h5>
    <p>{{ data[0].date }}</p>
  </div>
  <div class="container mt-4">
    <h5 @click="$router.push('/detail/1')">{{ data[1].title }}</h5>
    <p>{{ data[1].date }}</p>
  </div>
  <div @click="$router.push('/detail/2')" class="container mt-4">
    <h5>{{ data[2].title }}</h5>
    <p>{{ data[2].date }}</p>
  </div>
</template>

<script>
export default {
  name: "ListView",
  props: {
    data: Object,
  },
};
</script>

<style></style>
