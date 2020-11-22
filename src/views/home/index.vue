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
                    <a target="_parent" href="/">Portfolio</a>
                  </li>
                  <li>|</li>
                  <li class="nav-item">
                    <a target="_parent" href="scanner">Scanner Pick</a>
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


        <div id="g">
        <ul id="grid" class="grid cs-style-4">

            <li>
                <figure>
                    <img src="assets/img/photo/001.jpg" alt="img01">
                    <figcaption>
                        <h3>Foto</h3>
                        <span>Descripcion de foto</span>
                        <a href="#">Escuchar</a>
                    </figcaption>
                </figure>
            </li>

            <li>
                <figure>
                    <img src="assets/img/photo/002.jpg" alt="img02">
                    <figcaption>
                        <h3>Foto</h3>
                        <span>Descripcion de foto</span>
                        <a href="#">Escuchar</a>
                    </figcaption>
                </figure>
            </li>

            <li>
                <figure>
                    <img src="assets/img/photo/003.jpg" alt="img03">
                    <figcaption>
                        <h3>Foto</h3>
                        <span>Descripcion de foto</span>
                        <a href="#">Escuchar</a>
                    </figcaption>
                </figure>
            </li>

            <li>
                <figure>
                    <img src="assets/img/photo/004.jpg" alt="img04">
                    <figcaption>
                        <h3>Foto</h3>
                        <span>Descripcion de foto</span>
                        <a href="#">Escuchar</a>
                    </figcaption>
                </figure>
            </li>

            <li>
                <figure>
                    <img src="assets/img/photo/005.jpg" alt="img05">
                    <figcaption>
                        <h3>Foto</h3>
                        <span>Descripcion de foto</span>
                        <a href="#">Escuchar</a>
                    </figcaption>
                </figure>
            </li>

            <li>
                <figure>
                    <img src="assets/img/photo/006.jpg" alt="img06">
                    <figcaption>
                        <h3>Foto</h3>
                        <span>Descripcion de foto</span>
                        <a href="#">Escuchar</a>
                    </figcaption>
                </figure>
            </li>

            <li>
                <figure>
                    <img src="assets/img/photo/006.jpg" alt="img06">
                    <figcaption>
                        <h3>Foto</h3>
                        <span>Descripcion de foto</span>
                        <a href="#">Escuchar</a>
                    </figcaption>
                </figure>
            </li>


        </ul>

        <ul id="grid" class="grid cs-style-6">

            <li>
                <figure>
                    <img src="assets/img/photo/001.jpg" alt="img01">
                    <figcaption>
                        <h3>Foto</h3>
                        <span>Descripcion de foto</span>
                        <a href="#">Escuchar</a>
                    </figcaption>
                </figure>
            </li>

            <li>
                <figure>
                    <img src="assets/img/photo/002.jpg" alt="img02">
                    <figcaption>
                        <h3>Foto</h3>
                        <span>Descripcion de foto</span>
                        <a href="#">Escuchar</a>
                    </figcaption>
                </figure>
            </li>

            <li>
                <figure>
                    <img src="assets/img/photo/003.jpg" alt="img03">
                    <figcaption>
                        <h3>Foto</h3>
                        <span>Descripcion de foto</span>
                        <a href="#">Escuchar</a>
                    </figcaption>
                </figure>
            </li>

            <li>
                <figure>
                    <img src="assets/img/photo/004.jpg" alt="img04">
                    <figcaption>
                        <h3>Foto</h3>
                        <span>Descripcion de foto</span>
                        <a href="#">Escuchar</a>
                    </figcaption>
                </figure>
            </li>

            <li>
                <figure>
                    <img src="assets/img/photo/005.jpg" alt="img05">
                    <figcaption>
                        <h3>Foto</h3>
                        <span>Descripcion de foto</span>
                        <a href="#">Escuchar</a>
                    </figcaption>
                </figure>
            </li>

            <li>
                <figure>
                    <img src="assets/img/photo/006.jpg" alt="img06">
                    <figcaption>
                        <h3>Foto</h3>
                        <span>Descripcion de foto</span>
                        <a href="#">Escuchar</a>
                    </figcaption>
                </figure>
            </li>

            <li>
                <figure>
                    <img src="assets/img/photo/006.jpg" alt="img06">
                    <figcaption>
                        <h3>Foto</h3>
                        <span>Descripcion de foto</span>
                        <a href="#">Escuchar</a>
                    </figcaption>
                </figure>
            </li>


        </ul>
        </div>

    </div>
  </home-layout>
</template>

    
    <script src="./assets/js/modernizr.custom.js"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/1.11.1/jquery.js"></script>
    
        <style> 
            #g {
                overflow-y: visible;
                overflow-x: auto;
                white-space: nowrap;
                vertical-align: text-top;
                margin: 0;
                padding: 0;
                clear: both;
                border-spacing: 5px;
            }
            li{ padding:10px; }
        </style>

    <script src="./assets/js/toucheffects.js"></script>
    <script>
        jQuery(function($) {
            $.fn.hScroll = function(amount) {
                amount = amount || 120;
                $(this).bind("DOMMouseScroll mousewheel", function(event) {
                    var oEvent = event.originalEvent,
                        direction = oEvent.detail ? oEvent.detail * -amount : oEvent.wheelDelta,
                        position = $(this).scrollLeft();
                    position += direction > 0 ? -amount : amount;
                    $(this).scrollLeft(position);
                    event.preventDefault();
                })
            };
        });

        $(document).ready(function() {
            $('#g').hScroll(40); // You can pass (optionally) scrolling amount
        });
    </script>


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
