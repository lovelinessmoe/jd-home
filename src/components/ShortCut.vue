<template>
  <div class="shortcut">
    <div class="w">
      <ul class="fl">
        <li>
          <!--<svg class="icon" aria-hidden="true">
            <use xlink:href="#icon-icon-test"></use>
          </svg>-->
          <span>内蒙古</span>
        </li>
      </ul>
      <ul class="fr">
        <li v-for="(item, index) in bar" :key="index">
          <a
            href="item1.path"
            v-for="(item1, index1) in item.text"
            :key="'a-'+index1"
            :class="item1.id == '1_2' ? 'beRed' : ''"
            >{{ item1.name }}</a >
          <!--<svg v-for="(item1, index2) in item.text" :key="'svg-'+index2"  class="icon" aria-hidden="true">
            <use v-if="item1.id == '88' " xlink:href="#icon-ai-arrow-down"></use>
          </svg>-->
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name : 'ShortCut',
  data() {
    return {
      ischoose: 1,
      bar: [
        {
          id: "1",
          name: "bar-login",
          text: [
            {
              id: "1_1",
              name: "你好，请登录  ",
              path: "https://passport.jd.com/new/login.aspx",
            },
            {
              id: "1_2",
              name: " 免费注册",
              path: "https://reg.jd.com/reg/person",
            },
          ],
        },
        {
          id: "00",
          name: "",
        },
        {
          id: "2",
          name: "bar-text",
          text: [
            {
              id: "2_1",
              name: "我的订单",
              path: "",
            },
          ],
        },
        {
          id: "00",
          name: "",
        },
        {
          id: "3",
          name: "bar-text",
          text: [
            {
              id: "88",
              name: "我的京东",
              path: "",
            },
          ],
        },
        {
          id: "00",
          name: "",
        },
        {
          id: "4",
          name: "bar-text",
          text: [
            {
              id: "4_1",
              name: "京东会员",
              path: "",
            },
          ],
        },
        {
          id: "00",
          name: "",
        },
        {
          id: "5",
          name: "bar-text",
          text: [
            {
              id: "88",
              name: "企业采购",
              path: "",
            },
          ],
        },
        {
          id: "00",
          name: "",
        },
        {
          id: "6",
          name: "bar-text",
          text: [
            {
              id: "88",
              name: "客户服务",
              path: "",
            },
          ],
        },
        {
          id: "00",
          name: "",
        },
        {
          id: "7",
          name: "bar-text",
          text: [
            {
              id: "88",
              name: "网站导航",
              path: "",
            },
          ],
        },
        {
          id: "00",
          name: "",
        },
        {
          id: "8",
          name: "bar-text",
          text: [
            {
              id: "8_1",
              name: "手机京东",
              path: "",
            },
          ],
        },
      ],
    };
  },
  methods: {},
  mounted() {
    //  var redLi = document.querySelector(".fr").firstElementChild
  },
  components: {},
};
</script>

<style  scoped>
.icon {
  font-size: 6px;
  color: var(--darkgray);
  padding-left: 6px;
}
.shortcut {
  background-color: var(--gray);
  width: 100%;
  overflow: hidden;
}

.shortcut .w {
  height: 30px;
}

.fl {
  float: left;
}
.fl li {
  line-height: 30px;
  padding: 0 5px;
}
.fl li:hover {
  background-color: #fff;
}
.fl li .icon {
  color: red;
  font-size: 1.3rem;
  line-height: 30px;
  padding-right: 5px;
}
.fr {
  /* background-color: blue; */

  float: right;
}
.fr li {
  line-height: 30px;
  display: inline-block;
  /* padding: 0 10px; */
  /* border-left: 1px solid #000; */
}
.fr li a {
  color: var(--darkgray);
}
.fr li:nth-child(2n) {
  border-left: 2px solid var(--darkgray);
  width: 1px;
  height: 10px;
  margin-left: 12px;
  padding: 0 8px;
}
.beRed {
  color: red !important;
}
.fr li:nth-child(9) a {
  color: red;
}

</style>


