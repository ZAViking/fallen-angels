<script setup lang="ts">
    const isOpen = ref(false)
</script>

<style scoped>
  .button-container {
    display: flex; /* Enables flexbox */
    justify-content: flex-end; /* Aligns content to the right */
    padding-right: 20px; /* Adds padding from the right side */
  }
</style>

<template>
  <div class="button-container">
    <UButton color="gray" label="Your Guide" @click="isOpen = true" />

    <USlideover v-model="isOpen">
      <UCard
        class="flex flex-col flex-1"
        :ui="{ body: { base: 'flex-1' }, ring: '', divide: 'divide-y divide-gray-100 dark:divide-gray-800' }"
      >
        <template #header>
          <UButton 
            color="gray" 
            variant="ghost" 
            icon="i-heroicons-x-mark-20-solid" 
            class="-my-1" 
            @click="isOpen = false" 
          />

          <!-- <Placeholder class="h-8" /> -->
        </template>

          <!-- <Placeholder class="h-full" /> -->
          <UDivider
            label="Navigation"
            :ui="{ label: 'text-gray-500 dark:text-gray-400' }"
          />
          <NuxtLink to="/">Home</NuxtLink><br />
          <NuxtLink to="/Lessons/resources">Resources</NuxtLink><br />
          <NuxtLink to="/About">About</NuxtLink><br />

          <UDivider
            label="Success"
            :ui="{ label: 'text-gray-500 dark:text-gray-400' }"
          />
          <NuxtLink to="/Lessons/6-demands-for-success">6 Demands for Success</NuxtLink><br />
          <NuxtLink to="/Lessons/laws-in-life">Laws in Life</NuxtLink><br />

          <UDivider
            label="Lessons"
            :ui="{ label: 'text-gray-500 dark:text-gray-400' }"
          />
          <NuxtLink to="/Lessons/mind-decoder">Mind Decoder</NuxtLink><br />
          <NuxtLink to="/Lessons/six-morning-tasks">6 Morning Tasks</NuxtLink><br />
          <NuxtLink to="/Lessons/let-them-theory">The "Let Them Theory"</NuxtLink><br />
          <NuxtLink to="/Lessons/how-to-deal-with-difficult-people">Handling Difficult People</NuxtLink><br />
          <NuxtLink to="/Lessons/life-lessons-from-the-stoic">Life Lessons From The Stoic</NuxtLink><br />
          <NuxtLink to="/Lessons/quotes">Useful Quotes</NuxtLink><br />
          
          <UDivider
          label="The male mind"
          :ui="{ label: 'text-gray-500 dark:text-gray-400' }"
          />
          <NuxtLink to="/Lessons/male-mind">The Male Mind</NuxtLink><br />
          
          <UDivider
          label="The female mind"
          :ui="{ label: 'text-gray-500 dark:text-gray-400' }"
          />
          <!-- <NuxtLink to="/Lessons/">The Female Mind</NuxtLink><br /> -->
          
        <template #footer>
          <!-- <Placeholder class="h-8" /> -->
        </template>

      </UCard>
    </USlideover>
    
  </div>
</template>

