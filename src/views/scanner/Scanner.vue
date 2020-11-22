<template>
  <home-layout>
<div class="container">
        <!-- Top Navigation -->
        
      <!--Begin Nav-->  
      <div class="landing-page-nav">
          <headroom style="height:initial;">
            <nav>
              <div class="container d-flex align-items-center justify-content-between">
                <a class="navbar-logo pull-left" @click="scrollTo('#home')" href="javascript:;">
                  <span class="white"></span>
                  <span class="dark"></span>
                </a>
                <ul class="navbar-nav d-none d-lg-flex flex-row">
                  <li class="nav-item">
                    <a href="/">Portfolio</a>
                  </li>
                  <li>|</li>
                  <li class="nav-item">
                    <a href="scanner">Scanner Pick</a>
                  </li>
                  <li>|</li>
                  <li class="nav-item ">
                    <a  target="_parent"  href="buybook">Buy Book</a>
                  </li>
                  <li>|</li>
                  <li class="nav-item">
                    <a target="_parent" href="/user/login">Login</a>
                  </li>

                </ul>
              </div>
            </nav>
          </headroom>
        </div>
        <!--End Nav-->

        <div>

            Zone Scanner Image

        </div>    


           

    </div>
  </home-layout>
</template>

    
        <style> 
      
            li{ padding:10px; }
        </style>


<script>
import { headroom } from "vue-headroom";
import VueScrollTo from "vue-scrollto";
import HomeLayout from "../../layouts/HomeLayout";
import GlideComponent from "../../components/Carousel/GlideComponent";
import { adminRoot, buyUrl } from "../../constants/config";
const slideSettings = {
  type: "carousel",
  gap: 30,
  perView: 4,
  hideNav: true,
  peek: { before: 10, after: 10 },
  breakpoints: {
    "600": { perView: 1 },
    "992": { perView: 2 },
    "1200": { perView: 3 }
  }
};



const scrollOptions = {
  container: "body",
  easing: "ease-in",
  offset: -120,
  force: true,
  x: false,
  y: true
};

export default {
  components: {
    "home-layout": HomeLayout,
    "glide-component": GlideComponent,
    headroom: headroom
  },
  data() {
    return {
      showMobileMenu: false,
    };
  },
  methods: {
    onWindowResize() {
      // const homeRect = document
      //   .getElementById("homeRow")
      //   .getBoundingClientRect();
      // const homeSection = document.getElementById("sectionHome");
      // homeSection.style.backgroundPositionX = homeRect.x - 580 + "px";

      // const footerSection = document.getElementById("sectionFooter");
      // footerSection.style.backgroundPositionX =
      //   event.target.innerWidth - homeRect.x - 2000 + "px";

      // if (event.target.innerWidth >= 992) {
      //   this.showMobileMenu = false;
      // }
    },
    onWindowScroll() {
      this.showMobileMenu = false;
    },
    onWindowClick() {
      this.showMobileMenu = false;
    },

    scrollTo(target) {
      VueScrollTo.scrollTo(target, 200, scrollOptions);
    }
  },
  mounted() {
    document.body.classList.add("no-footer");
    window.addEventListener("scroll", this.onWindowScroll);
    window.addEventListener("resize", this.onWindowResize);
    window.addEventListener("click", this.onWindowClick);
  },
  beforeDestroy() {
    document.body.classList.remove("no-footer");
    window.removeEventListener("scroll", this.onWindowScroll);
    window.removeEventListener("resize", this.onWindowResize);
    window.removeEventListener("click", this.onWindowClick);
  }
};
</script>
