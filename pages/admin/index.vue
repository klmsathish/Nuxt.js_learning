<template>
  <div class="admin-page">
    <section class="new-post">
      <AppButton @click="$router.push('/admin/new-post')">Create Post</AppButton>
    </section>
    <section class="existing-posts">
      <h1>Existing Posts</h1>
      <PostList isAdmin />
    </section>
  </div>
</template>

<script>
import PostList from '@/components/posts/postList'
import AppButton from '@/components/ui/AppButton'
export default {
  components: {
    PostList
  },
  layout:'admin'
}
</script>



<style scoped>
.admin-page {
  padding: 20px;
}

.new-post {
  text-align: center;
  border-bottom: 2px solid #ccc;
  padding-bottom: 10px;
}

.existing-posts h1 {
  text-align: center;
}
</style>

 