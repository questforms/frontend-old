<script setup lang="ts">
import { ref } from 'vue'

defineProps<{ msg: string }>()

// import logo from '@/assets/images/logo.svg';
</script>

<template>
  <header class="header">
    <nav class="header__super-header">
      <ul class="super-header__list">
        <li class="super-header__item">First super header nav item</li>
      </ul>
    </nav>
    <nav class="header__main-nav">
      <a href="/" class="main-nav__logo">
        <img src="../assets/images/logo-main.svg" class="logo__image" alt="QuestForms" />
      </a>
      <ul class="main-nav__list">
        <li class="main-nav__item">First nav item</li>
        <li class="main-nav__item">Second nav item</li>
        <li class="main-nav__item">Third nav item</li>
        <li class="main-nav__item">Fourth nav item</li>
      </ul>
    </nav>
  </header>
</template>

<style scoped>
.card__button {
  background-color: var(--primary-color);
}

.header__super-header {
  background-color: black;
  color: white;
}

.header__main-nav {
  display: flex;
  flex-direction: row;
  padding: 1.5em;
  background-color: #fff;
}

.logo__image {
  height: 40px;
}

.main-nav__list {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(140px, 1fr));
  width: 100%;
}

.main-nav__item {
  list-style: none;
  text-align: center;
  line-height: 40px;
}
</style>
