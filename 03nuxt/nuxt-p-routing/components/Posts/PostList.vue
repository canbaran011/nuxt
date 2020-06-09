<template>
    <div>
        <section class="post-list">
        <PostPreview
          id="1"
          :is-admin="isAdmin"
          thumbnail="http://omargardens.com/blog/wp-content/uploads/2017/06/spring-in-nature-wide-wallpaper-603794.jpg"
          title="Hello Nature"
          previewText="This is the real nature sorrow"
        />
        <PostPreview
          id="1"
          :is-admin="isAdmin"
          thumbnail="http://omargardens.com/blog/wp-content/uploads/2017/06/spring-in-nature-wide-wallpaper-603794.jpg"
          title="Hello Nature Two"
          previewText="This is  2 the real nature sorrow"
        />
      </section>
    </div>
</template>
<script>
import PostPreview from "@/components/Posts/PostPreview.vue";

export default {
  components: {
    PostPreview
  },
  props: {
    isAdmin : {
      type : Boolean,
      default : false
    }
  }
};
</script>
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