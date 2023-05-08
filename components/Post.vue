<!--<template>-->
<!--  <NuxtLink :to='post.uri'>-->

<!--    <h2 class="font-semibold text-2xl">{{ post.title }}</h2>-->
<!--    <p>{{ new Date(post.date).toLocaleDateString() }}</p>-->

<!--  </NuxtLink>-->
<!--</template>-->

<!--<script setup lang="ts">-->
<!--const props = defineProps<{-->
<!--  post: Record<'title' | 'date' | 'excerpt' | 'uri', string>-->
<!--}>();-->
<!--</script>-->



<script lang="ts" setup>
defineProps<{
  title: string;
  excerpt?: string;
  image?: string;
  slug?: string;
}>();
</script>

<template>
  <h3 class="grid__content-title text-xl font-semibold mb-2">
    {{ title }}
  </h3>

  <NuxtLink
      v-if="slug"
      class="blog__readmore border-b-2 border-primary-500 inline-flex items-center"
      :to="`/${slug}`"
  >Read more

  </NuxtLink>
</template>