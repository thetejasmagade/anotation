<template>
  <nav class="fixed bg-white w-full">
    <NuxtLink to="/" class="flex items-center pl-2.5 mb-2 pt-2">
      <svg width="32" height="32" viewBox="0 0 24 24">
        <g
          fill="none"
          stroke="#ec4899"
          stroke-linecap="round"
          stroke-linejoin="round"
          stroke-width="2"
        >
          <path
            fill="url(#Gradient3)"
            fill-opacity=".3"
            d="M20 6V5C20 4.45 19.55 4 19 4H5C4.45 4 4 4.45 4 5V19C4 19.55 4.45 20 5 20H19C19.55 20 20 19.55 20 19zM8 8h8M8 12h8M8 16h5"
          >
            <animateMotion
              fill="freeze"
              calcMode="linear"
              dur="3.5s"
              path="M0 0l2-2"
              repeatCount="indefinite"
            />
          </path>
          <path
            stroke-dasharray="34"
            stroke-dashoffset="34"
            d="M2 6V21C2 21.55 2.45 22 3 22H18"
          >
            <animate
              fill="freeze"
              attributeName="stroke-dashoffset"
              dur="3.5s"
              values="34;68"
              repeatCount="indefinite"
            />
          </path>
        </g>
        <defs>
          <linearGradient id="Gradient3">
            <stop stop-color="#f9caaa" offset="0" />
            <stop stop-color="#f9caaa" offset="20%" />
            <stop stop-color="#f9ae7a" offset="20%" />
            <stop stop-color="#f9ae7a" offset="40%" />
            <stop stop-color="#f79959" offset="40%" />
            <stop stop-color="#f79959" offset="60%" />
            <stop stop-color="#f97821" offset="60%" />
            <stop stop-color="#fc9149" offset="80%" />
            <stop stop-color="#f97821" offset="80%" />
            <stop stop-color="#f97821" offset="100%" />
          </linearGradient>
        </defs>
      </svg>
      &nbsp;&nbsp;
      <span class="text-xl" v-if="!$device.isMobile">Anotation</span>
    </NuxtLink>
  </nav>
</template>

<script>
export default {};
</script>

<style>
</style>