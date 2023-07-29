<template>
  <div class="bg-gray-100">
    <div class="mx-auto max-w-7xl px-4 sm:px-6 lg:px-8">
      <div class="mx-auto max-w-2xl py-16 sm:py-24 lg:max-w-none lg:py-32">
        <h2 class="text-2xl font-bold text-gray-900">𝑺𝒌𝒊𝒍𝒍</h2>

        <div class="mt-6 space-y-12 lg:grid lg:grid-cols-3 lg:gap-x-6 lg:space-y-0">
          <div v-for="callout in callouts" :key="callout.name" class="group relative">
            <div class="relative h-80 w-full overflow-hidden rounded-lg bg-white sm:aspect-h-1 sm:aspect-w-2 lg:aspect-h-1 lg:aspect-w-1 group-hover:opacity-75 sm:h-64">
              <img :src="callout.imageSrc" :alt="callout.imageAlt" class="h-full w-full object-cover object-center" />
            </div>
            <center><h3 class="mt-6 text-sm text-gray-500" style="color: red;">
              <a :href="callout.href"><span class="absolute inset-0"></span>{{ callout.name }}</a>
            </h3>
            <p class="text-base font-semibold text-gray-900" style="color: black;">{{ callout.description }}</p></center>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script setup>
const callouts = [
  {
    name: 'UI & UX',
    description: 'Work from home accessories',
    imageSrc: '/public/picture/uiux.jpg',
  },
  {
    name: 'JavaScript',
    description: 'Work from home accessories',
    imageSrc: '/public/picture/js.png',
  },
  {
    name: 'Express',
    description: 'Journals and note-taking',
    imageSrc: '/public/picture/express.png',
  },
]
</script>