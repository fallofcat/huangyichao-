<template>
  <div class="homeHeader">
    <div class="homgHeader-top">
      <slot name='imgleft'></slot>
      <input type="search" class='search' placeholder="ajax·php·android">
      <slot name='imgright'></slot>
    </div>
    <div class="homgHeader-bottom">
      <ul>
        <li>
          <router-link to='/home/recommended'>推荐</router-link>
        </li>
        <li>
          <router-link to='/home/freeclass'>免费课程</router-link>
        </li>
        <li>
          <router-link to='/home/jobpath'>职业路径</router-link>
        </li>
        <li>
          <router-link to='/home/livebroadcastclass'>直播课程</router-link>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
  export default {
    mounted() {
      this.$router.push({
        path: '/home/recommended'
      })
    }
  }
</script>

<style scoped lang="less">
.homeHeader{
    height: 160/75rem;
}
  .homgHeader-top {
    padding-top: 20/75rem;
    display: flex;
    justify-content: center;
    align-items: center;

    .img {
      width: 35/75rem;
      height: 35/75rem;
    }

    .search {
      border: none;
      background: #ededee;
      width: 550/75rem;
      height: 55/75rem;
      border-radius: 100/75rem;
      text-indent: 1em;
      padding-right: 10/75rem;

      &::-webkit-input-placeholder {
        text-align: center;
      }
    }

    .imgright {
      padding-left: 28/75rem;
    }

    .imgleft {
      padding-right: 28/75rem;
    }
  }

  .homgHeader-bottom {
    ul {
      display: flex;

      li {
        flex: auto;
        text-align: center;
        font-size: 28/75rem;
        font-weight: bold;
        line-height: 84/75rem;

        a {
          color: black;
        }
      }
    }

  }
</style>
