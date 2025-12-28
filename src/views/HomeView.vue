<template>
  <div class="home-view">
    <div class="profile-container">
      <img src="/profile.png" alt="Foto de perfil" class="profile-image" />
      <h1 class="name">Sergi Rourera</h1>
      <router-link to="/cv" class="cv-button"> See my CV </router-link>
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  name: "HomeView",
});
</script>

<style scoped>
.home-view {
  display: flex;
  justify-content: center;
  align-items: center;
  min-height: 80vh;
  padding: 2rem;
}

.profile-container {
  text-align: center;
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 1.5rem;
}

.profile-image {
  width: 200px;
  height: 200px;
  border-radius: 50%;
  object-fit: cover;
  border: 4px solid #131930;
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
}

.name {
  color: #2c3e50;
  font-size: 2.5rem;
  margin: 0;
  font-weight: 600;
}

.cv-button {
  display: inline-block;
  padding: 12px 32px;
  background-color: #131930;
  color: white;
  text-decoration: none;
  border-radius: 8px;
  font-size: 1.1rem;
  font-weight: 500;
  transition: background-color 0.3s ease;
  cursor: pointer;
}

.cv-button:hover {
  background-color: #1a2332;
}
</style>
