<template>
  <div id="ranking-board">
    <div class="ranking-board-title">Data Title</div>
    <dv-scroll-ranking-board :config="config" />
  </div>
</template>

<script>
export default {
  name: 'RankingBoard',
  data () {
    return {
      config: {
        data: [
          {
            name: 'Data',
            value: 55
          },
          {
            name: 'Data',
            value: 120
          },
          {
            name: 'Data',
            value: 78
          },
          {
            name: 'Data',
            value: 66
          },
          {
            name: 'Data',
            value: 80
          },
          {
            name: 'Data',
            value: 45
          }
        ],
        rowNum: 6
      }
    }
  }
}
</script>

<style lang="less">
#ranking-board {
  width: 100%;
  height: 100%;
  position: relative;
  box-shadow: 0 0 3px blue;
  display: flex;
  flex-direction: column;
  background-color: rgba(6, 30, 93, 0.5);
  border-top: 2px solid rgba(1, 153, 209, .5);
  box-sizing: border-box;
  padding: 0px 30px;

  .ranking-board-title {
    height: 50px;
    display: flex;
    align-items: center;
    font-size: 20px;
  }

  .dv-scroll-ranking-board {
    flex: 1;
  }
}
</style>
