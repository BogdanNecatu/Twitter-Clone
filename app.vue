<template>
  <div :class="{ dark: darkMode }">
    <div class="bg-white dark:bg-dim-900">
      <div class="min-h-full">
        <div class="mx-auto grid grid-cols-12 sm:px-6 lg:max-w-7xl lg:gap-5 lg:px-8">
          <!-- Left sidebare -->
          <div class="xs-col-spa-1 hidden md:block xl:col-span-2">
            <div class="stiky top-0">
              <SidebarLeft />
            </div>
          </div>

          <!--Main content-->
          <!-- <main class="col-span-12 bg-red-300 col-span-8 md:col-span-8 xl:col-span-6">
            <h1>Hello</h1>
          </main> -->
          <!--Right sidebare-->
          <div class="col-span-12 bg-blue-400 md:col-span-3 md:block xl:col-span-4">
            <div class="stiky top-0">
              <SidebarRight />
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
const darkMode = ref(true)
</script>
