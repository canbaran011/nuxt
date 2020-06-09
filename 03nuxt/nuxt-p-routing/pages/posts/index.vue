<template>
  <div>
    <h2>Posts Page</h2>
    <div class="posts-page">
      <PostList />
    </div>
  </div>
</template>
<script>
import PostList from "@/components/Posts/PostList.vue";

export default {
  components: {
    PostList
  }
};
</script>

<style scoped>
.posts-page {
  display: flex;
  justify-content: center;
  align-items: center;
}
</style>
