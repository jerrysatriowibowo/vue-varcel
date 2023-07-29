<template>
    <div class="bg-white">
      <div class="mx-auto grid max-w-2xl grid-cols-1 items-center gap-x-8 gap-y-16 px-4 py-24 sm:px-6 sm:py-32 lg:max-w-7xl lg:grid-cols-2 lg:px-8">
        <div>
          <h2 class="text-3xl font-bold tracking-tight text-gray-900 sm:text-4xl" style="color: black;">𝑯𝒐𝒃𝒊</h2>
          <p class="mt-4 text-gray-500" style="color: black;">𝘋𝘪𝘣𝘢𝘸𝘢𝘩 𝘐𝘯𝘪 𝘈𝘥𝘢𝘭𝘢𝘩 𝘏𝘰𝘣𝘺 𝘠𝘢𝘯𝘨 𝘚𝘢𝘺𝘢 𝘔𝘪𝘯𝘢𝘵𝘪 𝘚𝘢𝘢𝘵 𝘐𝘯𝘪 𝘋𝘢𝘯 𝘠𝘢𝘯𝘨 𝘚𝘦𝘳𝘪𝘯𝘨 𝘚𝘢𝘺𝘢 𝘓𝘢𝘬𝘶𝘬𝘢𝘯.</p>
  
          <dl class="mt-16 grid grid-cols-1 gap-x-6 gap-y-10 sm:grid-cols-2 sm:gap-y-16 lg:gap-x-8">
            <div v-for="feature in features" :key="feature.name" class="border-t border-gray-200 pt-4">
              <dt class="font-medium text-gray-900" style="color: black;">{{ feature.name }}</dt>
              <dd class="mt-2 text-sm text-gray-500" style="color: black;">{{ feature.description }}</dd>
            </div>
          </dl>
        </div>
        <div class="grid grid-cols-2 grid-rows-2 gap-4 sm:gap-6 lg:gap-8">
          <img src="/public/picture/badminton.jpg" alt="Walnut card tray with white powder coated steel divider and 3 punchout holes." class="rounded-lg bg-gray-100" />
          <img src="/public/picture/bola.png" alt="Top down view of walnut card tray with embedded magnets and card groove." class="rounded-lg bg-gray-100" />
          <img src="/public/picture/game3.png" alt="Side of walnut card tray with card groove and recessed card area." class="rounded-lg bg-gray-100" />
          <img src="/public/picture/voly.png" alt="Walnut card tray filled with cards and card angled in dedicated groove." class="rounded-lg bg-gray-100" />
        </div>
      </div>
    </div>
</template>
<script setup>
const features = [
    { name: 'Sepak Bola', description: 'Saya Menyukai Sepak Bola Ketika Saya Masih Kecil' },
    { name: 'Bola Volly ', description: 'Saya Suka Bermain Volly Namun Ketika Hanya Perlombaan Saja'},
    { name: 'Bermain Games', description: 'Terkadang Ketika Saya Gabut Di Rumah Saya Lebih Memilih Bermain Game'},
    { name: 'Badminton', description: 'Badminton Adalah Salah Satu Olahraga Favorit Saya'},
]
</script>