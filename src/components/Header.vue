<template>
  <div class="header">
    <div class="logo">
      <img src="https://fakeimg.pl/100x50/?text=JustPlay"
           alt="">
      <p>
        闲玩
      </p>
    </div>
    <div class="search">
      <div class="search-option">
        <div>1</div>
        <div>2</div>
        <div>3</div>
      </div>
      <input type="text"
             name=""
             id=""
             placeholder="请输入要搜索的内容"
             class="search-content">
      <div class="search-button">
        搜索
      </div>
    </div>
    <div class="user">
      <img src="https://fakeimg.pl/50x50/?text=User"
           alt=""
           class="avatar">
      <div class="post">
        <div class="post-button">发布</div>
        <div class="post-options">
          <div class="option">我想出</div>
          <div class="option">我想买</div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: 'HeaderModal'
}
</script>

<style lang="scss" scoped>
.header {
    position: fixed;
    top: 0;
    left: 0;
    right: 0;

    border: 1px solid lightgray;
    height: 6rem;

    display: flex;
    flex-direction: row;
    justify-content: space-between;

    padding: 0 5rem;

    .logo {
        img {
            padding: 0.5rem;
            float: left;
            border-radius: 1rem;
        }

        p {
            float: right;
            line-height: 6rem;
            font-size: 2rem;
        }
    }

    .search {
        width: 50rem;
        height: 5rem;
        margin: 0.5rem 0;
        border: 1px solid lightgray;
        border-radius: 1rem;
        text-align: center;

        :focus {
            border: 1px solid #fefb05;
        }

        .search-option {
            float: left;
            display: none;
        }

        .search-content {
            line-height: 4.5rem;
            width: 40rem;
            display: inline-block;
            margin-left: 1rem;
            border: none;
            color: gray;
            outline: none;
        }

        .search-button {
            height: 4rem;
            width: 6rem;
            margin: 0.3rem 1rem;
            line-height: 4rem;
            border: 1px solid #fefb05;
            border-radius: 1rem;
            float: right;
            background-color: #fefb05;
        }
    }

    .user {
        .avatar {
            margin: 0.4rem 0;
            border-radius: 1rem;
        }

        .post {
            float: right;
            font-size: 1.5rem;
            border: 1px solid none;
            border-radius: 1rem;
            height: 4rem;
            width: 8rem;
            line-height: 4rem;
            margin: 0.6rem 1rem;
            padding: 0 0.5rem;
            background-color: #fefb05;
            color: #000;

            .post-options {
                display: none;
                position: absolute;
                border: 1px solid lightgray;
                border-radius: 0.5rem;
                width: 8rem;
                margin: 0.3rem -0.5rem;

                .option {
                    border-bottom: 1px solid lightgray;
                }
                .option:hover {
                    background-color: #000;
                    color: #fff;
                }
            }
        }

        .post:hover .post-options {
            display: block;
        }

        @keyframes slide-up {
            from {
                display: none;
            }
            to {
                display: inline-block;
            }
        }
    }
}
</style>
