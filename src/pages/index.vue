<script setup></script>

<script setup>
import userAuth from "../composable/useAuth";
const { isAuthenticated, user } = userAuth();
</script>

<template>
  <div
    class="
      flex flex-col
      items-center
      justify-center
      space-y-12
      min-h-screen-nonav
    "
  >
    <h2
      v-if="!isAuthenticated"
      class="text-6xl tracking-tighter font-bold text-purple-900 font-serif"
    >
      Welcome
    </h2>
    <h2 v-else class="text-6xl tracking-tighter font-bold font-serif">
      Welcome {{ user }}
    </h2>
    <img src="../assets/welcome.png" alt="Hello" />
  </div>
</template> 