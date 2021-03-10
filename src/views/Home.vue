<template>
  <div class="home">
    <div
      id="menu"
      @click="overlay = !overlay"
      :class="['hover_animation', overlay ? 'menu_close' : 'menu_open']"
      :data-mark="overlay"
    >
      <span></span>
      <span></span>
      <span></span>
    </div>
    <!-- <v-overlay
      :absolute="absolute"
      :value="overlay"
      :class="['navgation', overlay ? 'navgation_open' : 'navgation_close']"
    >
      <ul class="point">
        <li><a href="#">首页</a></li>
        <li><a href="article.html">博客</a></li>
        <li><a href="message.html">留言</a></li>
      </ul>
      <div class="logo"><a>Mr.Xu</a></div>
    </v-overlay> -->
    <div id="navgation" :class="['navgation', overlay ? 'navgation_open' : 'navgation_close']">
        <ul class="point">
            <li><a href="#">首页</a></li>
            <li><a href="article.html">博客</a></li>
            <li><a href="message.html">留言</a></li>
        </ul>
        <div class="logo"><a>Mr.XU</a></div>
    </div>

    <div class="section" id="section1">
      <div class="fp-tablecell">
        <div class="page1" >
          <div class="wow fadeInUp nav" data-wow-duration="2s">
            <h1>XZH-Blog</h1>
            <p>只要朝着一个方向努力，一切都会变得得心应手</p>
            <v-btn>Enter Blog</v-btn>
          </div>
          <a class="next wow fadeInUp" @click="nextPage" data-wow-duration="2s" ></a>
        </div>
      </div>
    </div>

    <div class="section" id="section2">
      <div class="fp-tablecell">
        <div class="page2">
          <div class="warp-box">
            <div class="new-article">
              <div class="inner wow fadeInDown" data-wow-delay=".2s">
                <h1>博客分类</h1>
                <p>
                  只要朝着一个方向努力
                  <br />一切都会变得得心应手
                </p>
              </div>
            </div>
            <v-row>
              <v-col >
                <div
                class="wow fadeInUp item "
                style="padding: 0 10px"
              >
                <div class="single-news">
                  <div class="news-head">
                    <img src="http://www.lzqcode.com/images/java.jpg" />
                    <a href="#" class="link"><i class="fa fa-link"></i></a>
                  </div>
                  <div class="news-content">
                    <h4>
                      <a href="#"> Java专栏 </a>
                    </h4>
                    <div class="date">2020年6月16日</div>
                    <p>
                      本专栏主要分享Java的各种常见问题，包括java学习路线，java基础，框架，微服务，项目，面试题，希望通过这些知识的分享能够提升自己的java水平
                    </p>
                    <a href="#" class="btn"> 阅读更多 </a>
                  </div>
                </div>
              </div>
              </v-col>
              <v-col >
                <div
                class="wow fadeInUp item "
                data-wow-delay=".2s"
                style="padding: 0 10px"
              >
                <div class="single-news">
                  <div class="news-head">
                    <img src="http://www.lzqcode.com/images/web.jpg" />
                    <a href="#" class="link"><i class="fa fa-link"></i></a>
                  </div>
                  <div class="news-content">
                    <h4>
                      <a href="#"> web前端专栏 </a>
                    </h4>
                    <div class="date">2020年6月16日</div>
                    <p>
                      本栏目主要分享关于web前端的学习路线，基础知识，常用框架，面试题，项目等等
                    </p>
                    <a href="#" class="btn"> 阅读更多 </a>
                  </div>
                </div>
              </div>
              </v-col>
              <v-col >
                <div
                class="wow fadeInUp item "
                data-wow-delay=".4s"
                style="padding: 0 10px"
              >
                <div class="single-news">
                  <div class="news-head">
                    <img src="http://www.lzqcode.com/images/dedecms.jpg" />
                    <a href="#" class="link"><i class="fa fa-link"></i></a>
                  </div>
                  <div class="news-content">
                    <h4>
                      <a href="#"> DeDeCMS专栏 </a>
                    </h4>
                    <div class="date">2020年6月16日</div>
                    <p>
                      本栏目主要介绍DeDeCMS网站内容管理系统，使用dede常见的问题，常用标签，插件，提供建站帮助
                    </p>
                    <a href="#" class="btn"> 阅读更多 </a>
                  </div>
                </div>
              </div>
              </v-col>
            </v-row>
          </div>
        </div>
      </div>
    </div>

    <div class="section" id="section3">
        <div class="fp-tablecell">
            <div class="page3">
                <div class="warp-box">
                    <div class="warp">
                        <div class="inner">
                            <div class="links">
                                <ul>
                                    <li class="wow fadeInLeft"><a href="#">关于</a></li>
                                    <li class="wow fadeInRight"><a href="#">+友情链接</a></li>
                                </ul>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>

    <div class="section" id="section4">
        <div class="fp-tablecell">
            <div class="page4">
                <div class="warp-box">
                    <div class="about">
                        <div class="inner">
                            <h1 class="wow fadeInLeft">XZH个人博客</h1>
                            <p class="wow fadeInRight">                         
                                   一天很短，开心了就笑，不开心了就过会儿再笑。
                            </p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
    
    <footer class="footer wow fadeInUp" id="contact">
        <div class="footer-top">
            <div class="container">
                <v-row>
                    <v-col>
                        <div class="single-widget about">
                            <div class="footer-logo">
                                <h2>XZH个人博客</h2>
                            </div>
                            <p>世界那么大，我想去看看</p>
                            <div class="button">
                                <v-btn href="#">About Me</v-btn>
                            </div>
                        </div>
                    </v-col>
                    <v-col >
                        <div class="single-widget">
                            <h2>相关链接</h2>
                            <ul class="social-icon">
                                <li class="active"><a href="#"><i class="fa fa-book"></i>博文</a></li>
                                <li class="active"><a href="#"><i class="fa fa-comments"></i>留言</a></li>
                                <li class="active"><a href="#"><i class="fa fa-share"></i>资源</a></li>
                                <li class="active"><a href="#"><i class="fa fa-snowflake-o"></i>日记</a></li>
                                <li class="active"><a href="#"><i class="fa fa-files-o"></i>归档</a></li>
                            </ul>                   
                        </div>
                    </v-col>
                    <v-col >
                        <div class="single-widget contact">
                            <h2>联系我</h2>
                            <ul class="list">
                                <li><i class="fa fa-map"></i>地址:深圳市南山区</li>
                                <li><i class="fa fa-qq"></i>QQ: 916813946 </li>
                                <li><i class="fa fa-envelope"></i>邮箱: 916813946@qq.com</li>
                            </ul>
                        </div>
                    </v-col>
                </v-row>
            </div>
        </div>
        <div class="copyright">
          <p>Copyright &copy; 2019-2020 ZQ个人博客 All Rights Reserved V.5.1.3 粤ICP备1231100号</p>       
        </div>  
    </footer>
  </div>
  
</template>

<script>
import {WOW} from "wowjs";
export default {
  name: "Home",
  data() {
    return {
      absolute: true,
      overlay: false,
    };
  },
  components: {},
  methods: {
    nextPage() {
      var scorllHeight = document.querySelector("#section2").offsetTop;
      window.scrollTo({
        top: scorllHeight,
        behavior: "smooth",
      });
    },
  },
  mounted() {
      var wow = new WOW({
        boxClass: 'wow',
	      animateClass: 'animated',
	      offset: 0,
	      mobile: true,
        live: false,        
      });
      wow.init();
  },
};
</script>

<style scoped>
@import url("../assets/css/index.css");
</style>