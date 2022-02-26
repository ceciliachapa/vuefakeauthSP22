<template>
  <div class="bg-pink-900 text-gray-100">
    <div class="container mx-auto flex items-center justify-between">
      <h1 class="tracking-tighter text-3xl font-thin">
        Vue<span class="font-normal">FakeAuth</span>
      </h1>
      <nav>
        <ul class="flex space-x-4">
          <router-link to="/">
            <li
              class="
                py-8
                px-4
                hover:cursor-pointer hover:bg-gray-400 hover:text-yellow-900
              "
            >
              Home
            </li></router-link
          >
          <router-link :to="{ name: 'About' }">
            <li
              class="
                py-8
                px-4
                hover:cursor-pointer hover:bg-gray-400 hover:text-yellow-900
              "
            >
              About
            </li></router-link
          >
          <router-link :to="{ path: '/login', name: 'Login' }">
            <li
              class="
                py-8
                px-4
                hover:cursor-pointer hover:bg-gray-400 hover:text-yellow-900
              "
            >
              Login
            </li></router-link
          >
          <router-link :to="{ name: 'Secret' }">
            <li
              class="
                py-8
                px-4
                hover:cursor-pointer hover:bg-gray-400 hover:text-yellow-900
              "
            >
              Secret
            </li></router-link
          >
        </ul>
      </nav>
    </div>
  </div>
</template>