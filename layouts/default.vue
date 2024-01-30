<template>
  <div class="flex flex-col h-screen">
    <!-- Header -->
    <header class="bg-white shadow">
      <div class="flex items-center justify-between p-4">
        <img src="https://placehold.co/100" alt="logo" class="h-10 w-10" />
        <input
          type="search"
          class="form-input flex-1 mx-4"
          placeholder="Search..."
        />
        <button class="btn">Button</button>
      </div>
    </header>

    <!-- Body -->
    <div class="flex flex-1 overflow-hidden">
      <!-- Sidebar -->
      <aside class="w-64 bg-gray-700 p-4 overflow-y-auto">
        <div>
          <h5 class="font-bold">Navigation</h5>
          <ul class="mt-4">
            <li><a href="#" class="btn btn-ghost">Link 1</a></li>
            <li><a href="#" class="btn btn-ghost">Link 2</a></li>
            <li><a href="#" class="btn btn-ghost">Link 3</a></li>
            <!-- ... other links ... -->
          </ul>
        </div>
        <button class="btn btn-ghost mt-auto">Logout</button>
      </aside>

      <!-- Main Content -->
      <main class="flex-1 p-4">
        <slot />
      </main>
    </div>
  </div>
</template>

<script setup></script>

<style>
/* Your styles here */
</style>
