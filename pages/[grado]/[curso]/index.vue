<template>
  <div>
    <h1>Grado: {{ grado }}</h1>
    <h2>Curso: {{ curso }}</h2>
    <p>Este es el contenido de la página del curso.</p>
    <h2>Lecciones</h2>
    <ul>
      <li>
        <NuxtLink :to="`/${grado}/${curso}/leccion1`">
          Lección 1
        </NuxtLink>
      </li>
      <li>
        <NuxtLink :to="`/${grado}/${curso}/leccion2`">
          Lección 2
        </NuxtLink>
      </li>
      <li>
        <NuxtLink :to="`/${grado}/${curso}/leccion3`">
          Lección 3
        </NuxtLink>
      </li>
    </ul>
  </div>
</template>
<script setup lang="ts">
const route = useRoute()

const grado = route.params.grado
const curso = route.params.curso
</script>