<template>
  <div class="home">
      <div class="splash-container">
            <div class="splash">
                <h1>Splendid Food</h1>
            </div>
        </div>

        <main class="wrapper">

            <h2>Recommended</h2>

            <div class="recommended">

                <div v-for="(product, i) in inventory.slice(0,3)" :key="product.id" class="card">
                </div>
            </div>

        </main>

  </div>
</template>

<script>

export default {
  name: 'HomeView',
  props: ['inventory', 'addToCart']
}
</script>
