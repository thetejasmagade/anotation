<template>
    <div>
      <v-app-bar color="#fff" flat
      >
      <v-app-bar-nav-icon @click="drawer = true"></v-app-bar-nav-icon>
      <svg width="32" height="32" viewBox="0 0 24 24" class="mx-auto">
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
      <button
        class="
          bg-gray-500
          hover:bg-gray-700
          text-white
          font-bold
          py-2
          px-4
          rounded-full
        "
      >
        Join
      </button>
      </v-app-bar>
  
      <v-navigation-drawer
        v-model="drawer"
        absolute
        temporary
      >
        <v-list
          nav
          dense
        >
          <v-list-item-group
            v-model="group"
            active-class="deep-purple--text text--accent-4"
          >
            <v-list-item>
              <v-list-item-icon>
                <v-icon>mdi-home</v-icon>
              </v-list-item-icon>
              <v-list-item-title>Home</v-list-item-title>
            </v-list-item>
  
            <v-list-item>
              <v-list-item-icon>
                <v-icon>mdi-account</v-icon>
              </v-list-item-icon>
              <v-list-item-title>Account</v-list-item-title>
            </v-list-item>
          </v-list-item-group>
        </v-list>
      </v-navigation-drawer>
      </div>
  </template>

<script>
    export default {
      data: () => ({
        drawer: false,
        group: null,
      }),
    }
  </script>