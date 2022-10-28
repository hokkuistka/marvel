<template>
  <h2 class="navbar navbar-dark bg-dark">
    <div class="container-fluid">
      <a class="navbar-brand">Марвел</a>
      <form class="d-flex">
        <input
          class="form-control me-2"
          type="search"
          placeholder="Введите запрос"
          aria-label="Search"
          v-model="search"
          @input = "changeSearch(search)"
        />
        <button class="btn btn-outline-warning" type="submit">Поиск</button>
      </form>
    </div>
  </h2>
</template>

<script>
export default {
  name: "AppHeader",
  props: ['changeSearch'],
  data() {
    return {
      search: "",
    };
  },
};
</script>

<style scoped>
</style>
