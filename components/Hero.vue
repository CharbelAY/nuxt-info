<template>
  <div class="Hero container">
    <div class="text-container">
      <h1 class="header">Find your Fire Extinguisher</h1>
      <p class="snippet">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Iste iusto illum quidem asperiores,
        cum nisi aperiam eius ipsa sapiente odit!</p>
      <button class="button btn">Start Looking</button>
    </div>
    <img class="image" src="~assets/svg/fire-extinguisher.svg" alt="fire extinguisher">
  </div>
</template>

<script>
import { mapState } from 'vuex'

export default {
  computed: {
    ...mapState([
      'data1',
      'data2'
    ])
  }
}
</script>

<style scoped>
.Hero {
  position: relative;
  display: flex;
  align-items: flex-start;
  justify-content: space-between;
}

.text-container {
  width: 50%;
  margin-top: 4rem;
}

.header {
  font-weight: 900;
  font-size: 5rem;
}

.snippet {
  color: grey;
  font-size: 1.25rem;
}

.image {
  width: 27.5rem;
  margin-top: 2rem;
  animation: transitionIn 2s;
}

.button {
  padding: 1rem 4rem;
  border-radius: 100rem;
  margin-top: 40px;
  background-color: rgb(231, 81, 43);
  color: white;
  width: 20rem;
  font-weight: 700;
  transition: 0.5s;
}

.button:hover {
  width: 21.5rem;
}

@keyframes transitionIn {
  0% {
    transform: translate(500px, 0);
  }
  100% {
    transform: translate(0, 0);

  }
}

</style>
