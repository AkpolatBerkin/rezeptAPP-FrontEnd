<template>
  <div>
    <h2>Rezept Liste</h2>
    <ul>
      <li v-for="rezept in rezepte" :key="rezept.id">
        {{ rezept.name }}
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  data() {
    return {
      rezepte: [
        { id: 1, name: 'Pasta Carbonara' },
        { id: 2, name: 'Tomatensuppe' },
        { id: 3, name: 'Pizza Margherita' }
      ]
    };
  }
};
</script>

<style scoped>
h2 {
  color: #42b983;
}
</style>
