<template>
  <div class="home-page">
    <section class="intro">
      <h1>yeah yuh</h1>
    </section>
    <section class="featured-posts">
      <PostPreview
        id="1"
        title="numba one"
        previewText="one bb"
        thumbnail="https://cdn0.tnwcdn.com/wp-content/blogs.dir/1/files/2016/03/WUFI-1-1100x655.png"
      />
      <PostPreview
        id="2"
        title="numba two"
        previewText="too bb"
        thumbnail="https://cdn0.tnwcdn.com/wp-content/blogs.dir/1/files/2016/03/WUFI-1-1100x655.png"
      />
      <PostPreview
        id="3"
        title="numba three"
        previewText="tree bb"
        thumbnail="https://cdn0.tnwcdn.com/wp-content/blogs.dir/1/files/2016/03/WUFI-1-1100x655.png"
      />
    </section>

  </div>
</template>
<script>
import PostPreview from '@/components/Posts/PostPreview'
export default {
  components:{
    PostPreview
  }
}
</script>

<style>
.intro {
  height: 300px;
  position: relative;
  padding: 30px;
  box-sizing: border-box;
  background-image: url('~assets/images/main-page-background.jpg');
  background-position: center;
  background-size: cover;
}

.intro h1 {
  position: absolute;
  top: 10%;
  left: 5%;
  width: 90%;
  font-size: 1.5rem;
  color: black;
  background-color: rgb(211, 211, 211);
  padding: 10px;
  border-radius: 10px;
  box-shadow: 3px 3px 3px black;
  box-sizing: border-box;
  border: 1px solid black;
}

@media (min-width: 768px) {
  .intro h1 {
    font-size: 2rem;
  }
}

.featured-posts {
  display: flex;
  padding: 20px;
  box-sizing: border-box;
  flex-wrap: wrap;
  align-items: center;
  justify-content: center;
}
</style>
