<template>
  <div class="menu">
    <button @click="toggleMenu">Toggle Menu</button>
    <ul v-if="isOpen" class="menu-list">
      <li v-for="(item, index) in items" :key="index">{{ item }}</li>
    </ul>
  </div>
</template>

<script>
export default {
  data() {
    return {
      isOpen: false,
      items: ['Home', 'About', 'Services', 'Contact']
    };
  },
  methods: {
    toggleMenu() {
      this.isOpen = !this.isOpen;
    }
  }
};
</script>

<style>
.menu-list {
  list-style: none;
  padding: 0;
}

.menu-list li {
  margin: 5px;
  cursor: pointer;
}
</style>