<template>
  <div>
    <h1>Pagina de la leccion</h1>
    <p>Esta es la página de lección.</p>
    <p>Grado: {{ grado }}</p>
    <p>Curso: {{ curso }}</p>
    <p>Lección: {{ leccion }}</p>
  </div>
</template>
<script setup lang="ts">
  const route = useRoute()

  const grado = route.params.grado
  const curso = route.params.curso
  const leccion = route.params.leccion
</script>