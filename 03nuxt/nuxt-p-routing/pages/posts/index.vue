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
  },
  asyncData(context) {
    return new Promise((resolve, reject) =>{
      setTimeout(() => {
      resolve({
        loadedPosts:[
          {
             id: "1",
             title: "First Post",
             previewText: "this is our first post",
             thumbnail:"http://omargardens.com/blog/wp-content/uploads/2017/06/spring-in-nature-wide-wallpaper-603794.jpg" 
          },
          {
              id: "2",
             title: "Second Post",
             previewText: "this is our second post",
             thumbnail:"http://omargardens.com/blog/wp-content/uploads/2017/06/spring-in-nature-wide-wallpaper-603794.jpg"
          }
        ]
      })
    }, 1500);
    })
    .then(data =>{
       return data;
    })
    .catch(e =>{
      context.error(new Error())
    })
    
  },
};
</script>

<style scoped>
.posts-page {
  display: flex;
  justify-content: center;
  align-items: center;
}
</style>
