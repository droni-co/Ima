<template>
  <div>
    <h1>Grados: {{ grado }}</h1>
    <p>Este es el contenido de la página de grados.</p>
    <ul>
      <li>
        <NuxtLink :to="`/${grado}/Matematicas`">
          Matematicas
        </NuxtLink>
      </li>
      <li>
        <NuxtLink :to="`/${grado}/Lengua`">
          Lengua
        </NuxtLink>
      </li>
      <li>
        <NuxtLink :to="`/${grado}/Ciencias`">
          Ciencias
        </NuxtLink>
      </li>
    </ul>
  </div>
</template>

<script setup lang="ts">
const route = useRoute()

const grado = route.params.grado
</script>