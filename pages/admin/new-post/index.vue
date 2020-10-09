<template>
    <div class = "admin-new-post-page">
        <section class = "new-post-form">
            <adminpostform />
        </section>
    </div>
</template>
<script>
import adminpostform from '@/components/admin/adminpostform'

export default {
  components: {
    adminpostform
  },
  layout:'admin'
}
</script>
<style scoped>
.new-post-form{
  width: 90%;
  margin: 20px auto;
}

@media (min-width: 768px) {
  .new-post-form{
    width: 500px;
  }
}
</style>