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
}
</script>