<script lang="ts" setup>
const {data: posts} = await useFetch<any>(
    "http://localhost/test.raiatec.com/wp-json/wp/v2/posts"
);

</script>
<template>
  <main>
    <div class="m-5">
      <div class="btn btn-success">Success</div>
    </div>
    <h1>
      elon musk !!!
    </h1>
    <Post
        v-for="post in posts"
        :key="post.id"
        :title="post.title.rendered"
        :excerpt="post.excerpt.rendered"
        :slug="post.slug"
    ></Post>
  </main>
</template>
