<template>
  <div class="h-16 flex items-center justify-center">
    <a href="#">
      <img
        src="https://tecdn.b-cdn.net/img/logo/mdb-transaprent-noshadows.png"
        style="width: 80px"
        alt=""
        loading="lazy"
      />
    </a>
  </div>
  <div>
    <VueItemMenu v-for="(menuItem, i) in menuItems" :key="i" :data="menuItem" />

    <div style="margin-bottom: 100px"></div>
  </div>
</template>

<script setup>
import VueItemMenu from "./VueItemMenu.vue";

const menuItems = [
  {
    name: "MENU",
    items: [
      {
        id: "g4as4",
        type: "urlLink", // urlLink or groupLink
        name: "Dashboard",
        path: "/",
        icon: `
        <svg
          fill="none"
          stroke="currentColor"
          stroke-linecap="round"
          stroke-linejoin="round"
          stroke-width="3"
          class="text-gray-300 w-4 h-4 mr-2"
          viewBox="0 0 24 24"
        >
          <path d="M22 11.08V12a10 10 0 11-5.93-9.14"></path>
          <path d="M22 4L12 14.01l-3-3"></path>
        </svg>
      `,
        data: [],
      },
    ],
  },
  {
    name: "CADASTROS",
    items: [
      {
        id: "1g32s",
        type: "urlLink", // urlLink or groupLink
        name: "Usuários",
        path: "/",
        icon: `
          <svg
            fill="none"
            stroke="currentColor"
            stroke-linecap="round"
            stroke-linejoin="round"
            stroke-width="2"
            class="text-gray-300 w-4 h-4 mr-2"
            viewBox="0 0 24 24"
          >
            <path d="M20 21v-2a4 4 0 00-4-4H8a4 4 0 00-4 4v2"></path>
            <circle cx="12" cy="7" r="4"></circle>
          </svg>
        `,
        data: [],
      },
      {
        id: "s7dj3",
        type: "urlLink", // urlLink or groupLink
        name: "Clientes",
        path: "/",
        icon: `
          <svg 
            xmlns="http://www.w3.org/2000/svg" 
            fill="none" 
            viewBox="0 0 24 24" 
            stroke-width="1.5" 
            stroke="currentColor" 
            class="text-gray-300 w-4 h-4 mr-2"
          >
            <path stroke-linecap="round" stroke-linejoin="round" d="M18 18.72a9.094 9.094 0 003.741-.479 3 3 0 00-4.682-2.72m.94 3.198l.001.031c0 .225-.012.447-.037.666A11.944 11.944 0 0112 21c-2.17 0-4.207-.576-5.963-1.584A6.062 6.062 0 016 18.719m12 0a5.971 5.971 0 00-.941-3.197m0 0A5.995 5.995 0 0012 12.75a5.995 5.995 0 00-5.058 2.772m0 0a3 3 0 00-4.681 2.72 8.986 8.986 0 003.74.477m.94-3.197a5.971 5.971 0 00-.94 3.197M15 6.75a3 3 0 11-6 0 3 3 0 016 0zm6 3a2.25 2.25 0 11-4.5 0 2.25 2.25 0 014.5 0zm-13.5 0a2.25 2.25 0 11-4.5 0 2.25 2.25 0 014.5 0z" />
          </svg>
        `,
        data: [],
      },
      {
        id: "a65sd",
        type: "urlLink", // urlLink or groupLink
        name: "Categorias",
        path: "/",
        icon: `
          <svg 
            xmlns="http://www.w3.org/2000/svg" 
            fill="none" 
            viewBox="0 0 24 24" 
            stroke-width="1.5" 
            stroke="currentColor"
            class="text-gray-300 w-4 h-4 mr-2"
          >
            <path stroke-linecap="round" stroke-linejoin="round" d="M16.5 8.25V6a2.25 2.25 0 00-2.25-2.25H6A2.25 2.25 0 003.75 6v8.25A2.25 2.25 0 006 16.5h2.25m8.25-8.25H18a2.25 2.25 0 012.25 2.25V18A2.25 2.25 0 0118 20.25h-7.5A2.25 2.25 0 018.25 18v-1.5m8.25-8.25h-6a2.25 2.25 0 00-2.25 2.25v6" />
          </svg>
        `,
        data: [],
      },
    ],
  },
  {
    name: "APP",
    items: [
      {
        id: "j8k76",
        type: "groupLink", // urlLink or groupLink
        name: "Relatórios",
        path: "#",
        icon: `
          <svg 
            xmlns="http://www.w3.org/2000/svg" 
            fill="none" 
            viewBox="0 0 24 24" 
            stroke-width="1.5" 
            stroke="currentColor" 
            class="text-gray-300 w-4 h-4 mr-2"
          >
            <path stroke-linecap="round" stroke-linejoin="round" d="M3.75 3v11.25A2.25 2.25 0 006 16.5h2.25M3.75 3h-1.5m1.5 0h16.5m0 0h1.5m-1.5 0v11.25A2.25 2.25 0 0118 16.5h-2.25m-7.5 0h7.5m-7.5 0l-1 3m8.5-3l1 3m0 0l.5 1.5m-.5-1.5h-9.5m0 0l-.5 1.5M9 11.25v1.5M12 9v3.75m3-6v6" />
          </svg>
        `,
        data: [
          {
            name: "DRE",
            path: "/",
          },
          {
            name: "Movimento Caixa",
            path: "/",
          },
          {
            name: "Planilha Resultados",
            path: "/",
          },
        ],
      },
      {
        id: "26sf3",
        type: "groupLink", // urlLink or groupLink
        name: "Mensagens",
        path: "#",
        icon: `
          <svg 
            xmlns="http://www.w3.org/2000/svg" 
            fill="none" 
            viewBox="0 0 24 24" 
            stroke-width="1.5" 
            stroke="currentColor" 
            class="text-gray-300 w-4 h-4 mr-2"
          >
            <path stroke-linecap="round" stroke-linejoin="round" d="M2.25 12.76c0 1.6 1.123 2.994 2.707 3.227 1.087.16 2.185.283 3.293.369V21l4.076-4.076a1.526 1.526 0 011.037-.443 48.282 48.282 0 005.68-.494c1.584-.233 2.707-1.626 2.707-3.228V6.741c0-1.602-1.123-2.995-2.707-3.228A48.394 48.394 0 0012 3c-2.392 0-4.744.175-7.043.513C3.373 3.746 2.25 5.14 2.25 6.741v6.018z" />
          </svg>
        `,
        data: [
          {
            name: "Internas",
            path: "/",
          },
          {
            name: "Whatsapp",
            path: "/",
          },
          {
            name: "E-mail",
            path: "/",
          },
        ],
      },
    ],
  },
  {
    name: "GERAIS",
    items: [
      {
        id: "1g32s",
        type: "urlLink", // urlLink or groupLink
        name: "Opção 01",
        path: "/",
        icon: `
          <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="text-gray-300 w-4 h-4 mr-2">
            <path stroke-linecap="round" stroke-linejoin="round" d="M17.593 3.322c1.1.128 1.907 1.077 1.907 2.185V21L12 17.25 4.5 21V5.507c0-1.108.806-2.057 1.907-2.185a48.507 48.507 0 0111.186 0z" />
          </svg>
        `,
        data: [],
      },
      {
        id: "s7dj3",
        type: "urlLink", // urlLink or groupLink
        name: "Opção 02",
        path: "/",
        icon: `
          <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="text-gray-300 w-4 h-4 mr-2">
            <path stroke-linecap="round" stroke-linejoin="round" d="M12 6.042A8.967 8.967 0 006 3.75c-1.052 0-2.062.18-3 .512v14.25A8.987 8.987 0 016 18c2.305 0 4.408.867 6 2.292m0-14.25a8.966 8.966 0 016-2.292c1.052 0 2.062.18 3 .512v14.25A8.987 8.987 0 0018 18a8.967 8.967 0 00-6 2.292m0-14.25v14.25" />
          </svg>
        `,
        data: [],
      },
      {
        id: "a65sd",
        type: "urlLink", // urlLink or groupLink
        name: "Opção 03",
        path: "/",
        icon: `
          <svg
            fill="none"
            stroke="currentColor"
            stroke-linecap="round"
            stroke-linejoin="round"
            stroke-width="2"
            class="text-gray-300 w-4 h-4 mr-2"
            viewBox="0 0 24 24"
          >
            <path
              d="M4 15s1-1 4-1 5 2 8 2 4-1 4-1V3s-1 1-4 1-5-2-8-2-4 1-4 1zM4 22v-7"
            ></path>
          </svg>
        `,
        data: [],
      },
    ],
  },
];
</script>
