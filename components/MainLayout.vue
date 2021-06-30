<template>
  <div class="main_page_layout">
    <!-- start preloader -->
    <div class="preloader">
      <div class="sk-spinner sk-spinner-wave">
        <div class="sk-rect1"></div>
        <div class="sk-rect2"></div>
        <div class="sk-rect3"></div>
        <div class="sk-rect4"></div>
        <div class="sk-rect5"></div>
      </div>
    </div>
    <!-- end preloader -->

    <!-- start header -->
    <header class="top-bar">
      <div class="container">
        <div class="row">
          <div class="col-md-3 col-sm-4 col-xs-12">
            <p><fa :icon="['fas', 'phone']" class="mr-2 top_bar_icon text-primary"/><span class="mr-2 font-weight-bold text_name"> Phone</span><span class="text_name">01828-96 32 35</span></p>
          </div>
          <div class="col-md-3 col-sm-4 col-xs-12">
            <p class=""><fa :icon="['fas', 'envelope']" class="mr-2 top_bar_icon text-primary"/><span class="mr-2 font-weight-bold text_name"> Email</span><span class="text_email font-weight-bold">smauhp@gmail.com</span></p>
          </div>
          <div class="col-md-5 col-sm-4 col-xs-12">
            <ul class="social_icon">
              <li class="social_icon_list"><span class="text-capitalize">find me on</span></li>
              <li class="social_icon_list"><a href="https://www.facebook.com/Asraf-Porag-108590421474289" target="_blank"><fa :icon="['fab', 'facebook']" class="social_icon_icon"/></a></li>
              <li class="social_icon_list"><a href="#" target="_blank"><fa :icon="['fab', 'twitter']" class="social_icon_icon"/></a></li>
              <li class="social_icon_list"><a href="https://www.instagram.com/asrafporag/" target="_blank"><fa :icon="['fab', 'instagram']" class="social_icon_icon"/></a></li>
              <li class="social_icon_list"><a href="https://www.linkedin.com/in/asrafporag" target="_blank"><fa :icon="['fab', 'linkedin']" class="social_icon_icon"/></a></li>
              <li class="social_icon_list"><a href="https://github.com/AP-Porag" target="_blank"><fa :icon="['fab', 'github']" class="social_icon_icon"/></a></li>
            </ul>
          </div>
        </div>
      </div>
    </header>
    <!-- end header -->

    <!-- start navigation -->
    <div class="navigation_bar">
      <b-navbar class="container" toggleable="lg" type="dark">
        <b-navbar-brand href="https://asrafporag.netlify.app" target="_blank">S. Asraf Porag</b-navbar-brand>

        <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

        <b-collapse id="nav-collapse" is-nav>

          <!-- Right aligned nav items -->
          <b-navbar-nav class="ml-auto">
            <b-nav-item href="#home" v-b-modal.modal-xl>Home</b-nav-item>
            <ModalMeComponent/>
            <b-nav-item href="#service">Service</b-nav-item>
            <b-nav-item href="#portfolio">Portfolio</b-nav-item>
            <b-nav-item to="/skills">Skills</b-nav-item>
            <ModalExperienceComponent/>
            <ModalEducationComponent/>
<!--            <b-nav-item href="#testimonial">Testimonial</b-nav-item>-->
            <b-nav-item href="#contact">Contact</b-nav-item>
          </b-navbar-nav>
        </b-collapse>
      </b-navbar>
    </div>
    <!-- end navigation -->

    <!-- start home -->
    <section id="home">
      <div class="content-block" id="header">
        <div id="overlay-1">

          <div class="middle text-center clearfix">
            <div class="container">
              <div class="row">
                <div class="col-md-4 offset-md-4">
                  <div class="about-left ">
                    <img src="~/assets/images/3L-1.jpg" class="img-fluid" alt="asraf porag">
                  </div>
                </div>
              </div>
              <h1 class="pro-name text-capitalize">full stack developer</h1>
              <p class="tagline text-capitalize">Php | Laravel | Node | react | Vue</p>
              <div class="skills">

              </div>  <!-- skills -->
              <a href="#contact" class="btn btn-lg btn-hire wow animated zoomIn">Hire Me</a>
            </div>  <!-- container -->
          </div>  <!-- middle -->
        </div>  <!-- overlay-1 -->
      </div>
    </section>
    <!-- end home -->

    <!-- start service -->
    <section id="service" class="service-area">
      <div class="container">
        <h2 class="block_title"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">Services</font></font></h2>
        <div class="row">
          <div class="col-md-3 col-sm-6">
            <div class="services">
              <div class="service-wrap">
                <i class="pe-7s-science pe-dj pe-va"></i>
                <h3><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">Creative ideas</font></font></h3>
                <p><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">Lorem ipsum dolor sit amet, consectetur adipiscing elit. </font><font style="vertical-align: inherit;">Snacks, please.</font></font></p>
              </div>
            </div>

          </div>
          <div class="col-md-3 col-sm-6">
            <div class="services">
              <div class="service-wrap">
                <i class="pe-7s-monitor pe-dj pe-va"></i>
                <h3><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">responsive Design</font></font></h3>
                <p><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">Lorem ipsum dolor sit amet, consectetur adipiscing elit. </font><font style="vertical-align: inherit;">Snacks, please.</font></font></p>
              </div>
            </div>
          </div>
          <div class="col-md-3 col-sm-6">
            <div class="services">
              <div class="service-wrap">
                <i class="pe-7s-edit pe-dj pe-va"></i>
                <h3><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">Clean and nice</font></font></h3>
                <p><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">Lorem ipsum dolor sit amet, consectetur adipiscing elit. </font><font style="vertical-align: inherit;">Snacks, please.</font></font></p>
              </div>
            </div>
          </div>
          <div class="col-md-3 col-sm-6">
            <div class="services">
              <div class="service-wrap">
                <i class="pe-7s-config pe-dj pe-va"></i>
                <h3><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">Support</font></font></h3>
                <p><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">Lorem ipsum dolor sit amet, consectetur adipiscing elit. </font><font style="vertical-align: inherit;">Snacks, please.</font></font></p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
    <!-- end service -->

    <!-- start portfolio -->
    <section id="portfolio" class="service-area">
      <div class="container-fluid">
        <div class="container">
          <div class="row">
            <div class="col-md-12">
              <h2 class="block_title"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">My Latest Work</font></font></h2>
            </div>
          </div>
        </div>
        <div class="row">
<!--          single work box start-->
          <div class="col-md-3 mb-4">
            <div class="work_box">
              <div class="work_details">
                <img src="~/assets/images/portfolio-img1.jpg" alt="" class="img-fluid">
                <div class="work_overlay_small">
                  <h6>Application</h6>
                  <h5>Project Name</h5>
                </div>
                <div class="work_overlay_full">
                  <h5 class="text-capitalize text-white text-center">Project Name</h5>
                  <div class="link_icon_box d-flex justify-content-between">
                    <fa :icon="['fas', 'envelope']" class="mr-2 top_bar_icon text-primary"/>
                    <fa :icon="['fas', 'envelope']" class="mr-2 top_bar_icon text-primary"/>
                    <fa :icon="['fas', 'envelope']" class="mr-2 top_bar_icon text-primary"/>
                  </div>
                </div>
              </div>
            </div>
          </div>
<!--          single work box end-->

          <!--          single work box start-->
          <div class="col-md-3 mb-4">
            <div class="work_box">
              <div class="work_details">
                <img src="~/assets/images/portfolio-img1.jpg" alt="" class="img-fluid">
                <div class="work_overlay_small">
                  <h6>Application</h6>
                  <h5>Project Name</h5>
                </div>
                <div class="work_overlay_full">
                  <h5 class="text-capitalize text-white text-center">Project Name</h5>
                  <div class="link_icon_box d-flex justify-content-between">
                    <fa :icon="['fas', 'envelope']" class="mr-2 top_bar_icon text-primary"/>
                    <fa :icon="['fas', 'envelope']" class="mr-2 top_bar_icon text-primary"/>
                    <fa :icon="['fas', 'envelope']" class="mr-2 top_bar_icon text-primary"/>
                  </div>
                </div>
              </div>
            </div>
          </div>
          <!--          single work box end-->

          <!--          single work box start-->
          <div class="col-md-3 mb-4">
            <div class="work_box">
              <div class="work_details">
                <img src="~/assets/images/portfolio-img1.jpg" alt="" class="img-fluid">
                <div class="work_overlay_small">
                  <h6>Application</h6>
                  <h5>Project Name</h5>
                </div>
                <div class="work_overlay_full">
                  <h5 class="text-capitalize text-white text-center">Project Name</h5>
                  <div class="link_icon_box d-flex justify-content-between">
                    <fa :icon="['fas', 'envelope']" class="mr-2 top_bar_icon text-primary"/>
                    <fa :icon="['fas', 'envelope']" class="mr-2 top_bar_icon text-primary"/>
                    <fa :icon="['fas', 'envelope']" class="mr-2 top_bar_icon text-primary"/>
                  </div>
                </div>
              </div>
            </div>
          </div>
          <!--          single work box end-->

          <!--          single work box start-->
          <div class="col-md-3 mb-4">
            <div class="work_box">
              <div class="work_details">
                <img src="~/assets/images/portfolio-img1.jpg" alt="" class="img-fluid">
                <div class="work_overlay_small">
                  <h6>Application</h6>
                  <h5>Project Name</h5>
                </div>
                <div class="work_overlay_full">
                  <h5 class="text-capitalize text-white text-center">Project Name</h5>
                  <div class="link_icon_box d-flex justify-content-between">
                    <fa :icon="['fas', 'envelope']" class="mr-2 top_bar_icon text-primary"/>
                    <fa :icon="['fas', 'envelope']" class="mr-2 top_bar_icon text-primary"/>
                    <fa :icon="['fas', 'envelope']" class="mr-2 top_bar_icon text-primary"/>
                  </div>
                </div>
              </div>
            </div>
          </div>
          <!--          single work box end-->

          <!--          single work box start-->
          <div class="col-md-3 mb-4">
            <div class="work_box">
              <div class="work_details">
                <img src="~/assets/images/portfolio-img1.jpg" alt="" class="img-fluid">
                <div class="work_overlay_small">
                  <h6>Application</h6>
                  <h5>Project Name</h5>
                </div>
                <div class="work_overlay_full">
                  <h5 class="text-capitalize text-white text-center">Project Name</h5>
                  <div class="link_icon_box d-flex justify-content-between">
                    <fa :icon="['fas', 'envelope']" class="mr-2 top_bar_icon text-primary"/>
                    <fa :icon="['fas', 'envelope']" class="mr-2 top_bar_icon text-primary"/>
                    <fa :icon="['fas', 'envelope']" class="mr-2 top_bar_icon text-primary"/>
                  </div>
                </div>
              </div>
            </div>
          </div>
          <!--          single work box end-->

          <!--          single work box start-->
          <div class="col-md-3">
            <div class="work_box">
              <div class="work_details">
                <img src="~/assets/images/portfolio-img1.jpg" alt="" class="img-fluid">
                <div class="work_overlay_small">
                  <h6>Application</h6>
                  <h5>Project Name</h5>
                </div>
                <div class="work_overlay_full">
                  <h5 class="text-capitalize text-white text-center">Project Name</h5>
                  <div class="link_icon_box d-flex justify-content-between">
                    <fa :icon="['fas', 'envelope']" class="mr-2 top_bar_icon text-primary"/>
                    <fa :icon="['fas', 'envelope']" class="mr-2 top_bar_icon text-primary"/>
                    <fa :icon="['fas', 'envelope']" class="mr-2 top_bar_icon text-primary"/>
                  </div>
                </div>
              </div>
            </div>
          </div>
          <!--          single work box end-->

          <!--          single work box start-->
          <div class="col-md-3 mb-4">
            <div class="work_box">
              <div class="work_details">
                <img src="~/assets/images/portfolio-img1.jpg" alt="" class="img-fluid">
                <div class="work_overlay_small">
                  <h6>Application</h6>
                  <h5>Project Name</h5>
                </div>
                <div class="work_overlay_full">
                  <h5 class="text-capitalize text-white text-center">Project Name</h5>
                  <div class="link_icon_box d-flex justify-content-between">
                    <fa :icon="['fas', 'envelope']" class="mr-2 top_bar_icon text-primary"/>
                    <fa :icon="['fas', 'envelope']" class="mr-2 top_bar_icon text-primary"/>
                    <fa :icon="['fas', 'envelope']" class="mr-2 top_bar_icon text-primary"/>
                  </div>
                </div>
              </div>
            </div>
          </div>
          <!--          single work box end-->

          <!--          single work box start-->
          <div class="col-md-3 mb-4">
            <div class="work_box">
              <div class="work_details">
                <img src="~/assets/images/portfolio-img1.jpg" alt="" class="img-fluid">
                <div class="work_overlay_small">
                  <h6>Application</h6>
                  <h5>Project Name</h5>
                </div>
                <div class="work_overlay_full">
                  <h5 class="text-capitalize text-white text-center">Project Name</h5>
                  <div class="link_icon_box d-flex justify-content-between">
                    <fa :icon="['fas', 'envelope']" class="mr-2 top_bar_icon text-primary"/>
                    <fa :icon="['fas', 'envelope']" class="mr-2 top_bar_icon text-primary"/>
                    <fa :icon="['fas', 'envelope']" class="mr-2 top_bar_icon text-primary"/>
                  </div>
                </div>
              </div>
            </div>
          </div>
          <!--          single work box end-->
        </div>
      </div>
    </section>
    <!-- end portfolio -->

    <!-- start testimonial -->
<!--    <section id="testimonial" class="service-area">-->
<!--      <div class="container">-->
<!--        <h2 class="block_title"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">Testimonial</font></font></h2>-->
<!--        <div class="row">-->
<!--          <div class="col-md-12">-->
<!--            <TestimonialSliderComponent/>-->
<!--          </div>-->
<!--        </div>-->
<!--      </div>-->
<!--    </section>-->
    <!-- end testimonial -->

    <!-- start contact -->
    <section id="contact" class="contact_area">
      <div class="contact_overlay">
        <div class="container">
          <h2 class="block_title"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">Get In Touch</font></font></h2>
          <div class="row">
            <div class="col-md-6 contact-left">
              <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3023.9503398796587!2d-73.9940307!3d40.719109700000004!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x89c25a27e2f24131%3A0x64ffc98d24069f02!2sCANADA!5e0!3m2!1sen!2sin!4v1441710758555" allowfullscreen="true" style="height: 100%;width: 100%;"></iframe>
            </div>
            <div class="col-md-6 contact-right">
              <form action="#" method="post">
                <div class="styled-input agile-styled-input-top">
                  <input type="text" class="text_input" name="Name" required="" placeholder="Name">
                  <span></span>
                </div>
                <div class="styled-input">
                  <input type="text" name="Email" required="" placeholder="Email">
                  <span></span>
                </div>
                <div class="styled-input">
                  <input type="text" name="Subject" required="" placeholder="Subject">
                  <span></span>
                </div>
                <div class="styled-input"><grammarly-extension data-grammarly-shadow-root="true" style="position: absolute; top: 0px; left: 0px; pointer-events: none;" class="cGcvT"></grammarly-extension><grammarly-extension data-grammarly-shadow-root="true" style="position: absolute; top: 0px; left: 0px; pointer-events: none;" class="cGcvT"></grammarly-extension>
                  <textarea name="Message" required="" spellcheck="false" placeholder="Message"></textarea>
                  <span></span>
                </div>
                <b-btn class="contact_send_btn">Send</b-btn>
              </form>
            </div>
          </div>
        </div>
      </div>
    </section>
    <!-- end contact -->

    <!-- start copyright -->
    <footer id="copyright" class="footer">
      <div class="container">
        <div class="row">
          <div class="col-md-12 text-center">
            <p class="pt-3">
              All Rights Reserved : Copyright &copy; 2021 S. Asraf Porag</p>
          </div>
        </div>
      </div>
    </footer>
    <!-- end copyright -->

  </div>
</template>

<script>
import ModalMeComponent from "~/components/ModalMeComponent";
import ModalSkillsComponent from "~/components/ModalSkillsComponent";
import ModalExperienceComponent from "~/components/ModalExperienceComponent";
import ModalEducationComponent from "~/components/ModalEducationComponent";
import TestimonialSliderComponent from "~/components/TestimonialSliderComponent";
export default {
  name: "MainLayout",
  components: {
    TestimonialSliderComponent,
    ModalEducationComponent, ModalExperienceComponent, ModalSkillsComponent, ModalMeComponent}
}
</script>

<style scoped>

</style>
