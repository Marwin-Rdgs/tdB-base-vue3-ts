<template>
  <nav>
    <h4 class="text-xl">
      <Bars3Icon class="inline-block h-5 w-5 text-blue-500" />
      menu (dans <code class="font-mono">/src/App.vue</code>)
    </h4>
    <ul>
      <li>
        <router-link class="text-red-600 underline" to="/">
          lien vers
          <code class="font-mono">/src/pages/index.vue</code>
        </router-link>
      </li>
      <li>
        <router-link class="text-red-600 underline" to="/simple">
          <h2>lien vers Page Simple</h2>
        </router-link>
      </li>
      <li>
        <router-link class="text-red-600 underline" to="/liste">
          <h2>lien vers Page Liste</h2>
        </router-link>
      </li>
      <li>
        <router-link class="text-red-600 underline" to="/liste-fetch">
          <h2>lien vers Page Liste-fetch</h2>
        </router-link>
      </li>

    </ul>
  </nav>

  <!-- Affiche les pages -->
 <Suspense> <router-view class="m-2 border-2 p-2" /></Suspense>
</template>

<script setup lang="ts">
import { Bars3Icon } from '@heroicons/vue/20/solid'
</script>
