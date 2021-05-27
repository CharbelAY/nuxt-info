<template>
  <nav class="navbar navbar-expand-lg navbar-dark bg-dark">
    <NuxtLink class="navbar-brand" to="/">Fire Thingi</NuxtLink>
    <button
      class="navbar-toggler"
      type="button"
      data-toggle="collapse"
      data-target="#navbarSupportedContent"
      aria-controls="navbarSupportedContent"
      aria-expanded="false"
      aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>

    <div class="collapse navbar-collapse" id="navbarSupportedContent">
      <ul class="navbar-nav ml-auto">
        <li class="nav-item">
          <NuxtLink class="nav-link" to="/products">Products </NuxtLink>
        </li>
        <li class="nav-item">
          <NuxtLink class="nav-link" to="/my-items">My Items</NuxtLink>
        </li>
      </ul>
    </div>
  </nav>
</template>

<script>
export default {
  name: 'Nav'
}
</script>

<style scoped>

</style>
