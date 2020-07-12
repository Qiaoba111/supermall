<template>
  <div>
    <div v-if="Object.keys(commentInfo).length !==0" class="comment-info">
      <div class="info-header">
        <div class="header-title">用户评价</div>
        <div class="header-more">更多
          <i class="arrow-right"></i>
        </div>
        <div class="info-user">
          <img src="commentInfo.user.avatar" alt="">
          <span>{{commentInfo.user.uname}}</span>
        </div>
      </div>

    </div>
  </div>
</template>
<script>
export default {
  name:"DetailCommentInfo",
  props:{
    commentInfo:{
      type:Object,
      default(){
        return{}
      }
    }
  }
}
</script>
<style scoped>

</style>