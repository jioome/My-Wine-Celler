<template>
  <div class="w-container">
    <Title :main-title="mainTitle" />
    <div class="main-content">
      <div class="board">
        <div v-for="(item,idx) in cards" :key="idx" class="board__card has-background-primary-light">hello</div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      mainTitle: '랜덤 피드',
      cards: [
        { title: '안녕하세요', content: '이런 와인이 있습니다.' },
        { title: '안녕하세요', content: '이런 와인이 있습니다.' },
        { title: '안녕하세요', content: '이런 와인이 있습니다.' },
        { title: '안녕하세요', content: '이런 와인이 있습니다.' },
        { title: '안녕하세요', content: '이런 와인이 있습니다.' },
      ],
    }
  },
}
</script>

<style lang="scss" scoped>
.board {
  overflow: auto;
  &__card {
    width: 90%;
    border-radius: 8px;
    margin: 4% auto 4% auto;
    min-height: 10rem;
    height: 15rem;
    padding: 1rem;
    box-shadow: 2px 2px 5px $base-color;
  }
}
</style>
