<template>
  <NuxtLayout>
    <Navbar />  
    <NuxtPage />
  </NuxtLayout>  
</template>

<style>
  .container {
    /* Aqui adicionamos margin auto para os containers já que o tailwind não faz isso automaticamente */
    /* também damos uma largura máxima de 1024px para a tela */
    @apply mx-auto max-w-5xl px-10 sm:px-0
  }
</style>
