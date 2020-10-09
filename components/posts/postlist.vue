<template>
    <section class = "post-list">
        <post 
        id ="1"
        :is-admin="isAdmin"          
        thumbnail = "https://media-exp1.licdn.com/dms/image/C5603AQGcYrRP2TnVtg/profile-displayphoto-shrink_400_400/0?e=1607558400&v=beta&t=m854Fs4ZWAaSsXUIoNwKZ-5qhEBEZEks9wgwhRvluIw"
        title = "Duck Boy"
        previewtext = "Backend Ready"/>
        <post 
        id ="2"
        :is-admin="isAdmin"
        thumbnail = "https://media-exp1.licdn.com/dms/image/C4E03AQFbt4dTR5HhcQ/profile-displayphoto-shrink_400_400/0?e=1607558400&v=beta&t=sjgvIOYehHVwol-tAz0vokNcGCvPLi0TXD-K3pdnu0g"
        title = "Playing with julia"
        previewtext = "CSS king"/>
      </section>
</template>
<style scoped>
.post-list {
  display: flex;
  padding: 20px;
  box-sizing: border-box;
  flex-wrap: wrap;
  align-items: center;
  justify-content: center;
}
</style>
<script>
import post from '~/components/posts/postpreview'
export default {
  components:{
  post
},
props:{
  isAdmin:{
    type:Boolean,
    default:false
  } 
}

}
</script>
