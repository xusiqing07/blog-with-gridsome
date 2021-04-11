<template>
  <div>
    <h1>{{$page.post.title}}</h1>
  </div>
</template>

<page-query>
query ($id: ID) {
  post: strapiTag (id: $id) {
    id
    title
    posts {
      id
      title
      content
    }
  }
}
</page-query>

<script>
export default {

}
</script>

<style>

</style>