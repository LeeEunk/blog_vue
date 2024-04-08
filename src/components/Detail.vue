<template>
  <h4 class="container mt-4">상세 번호 : {{ $route.params.id }}</h4>
  <div class="container mt-4">
    <div class="card" style="width: 18rem">
      <div class="card-body">
        <h5 class="card-title">{{ data[$route.params.id].title }}</h5>
        <h6 class="card-subtitle mb-2 text-body-secondary">
          {{ data[$route.params.id].date }}
        </h6>
        <p class="card-text">{{ data[$route.params.id].content }}</p>
      </div>
    </div>
    <router-view></router-view>
  </div>
</template>

<script>
export default {
  name: "DetailView",
  props: {
    data: Object,
  },
};
</script>

<style></style>
