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
            <b-nav-item href="#" v-b-modal.modal-xl>Home</b-nav-item>
            <ModalMeComponent/>
            <b-nav-item href="#">Service</b-nav-item>
            <b-nav-item href="#">Portfolio</b-nav-item>
            <ModalSkillsComponent/>
            <ModalExperienceComponent/>
            <ModalEducationComponent/>
            <b-nav-item href="#">Testimonial</b-nav-item>
            <b-nav-item href="#">Contact</b-nav-item>
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

    <!-- start about -->
    <section id="about">
      <div class="container">
        <div class="row">
          <div class="col-md-12">
            <h2 class="wow bounceIn" data-wow-offset="50" data-wow-delay="0.3s">WE ARE <span>AWESOME</span></h2>
          </div>
          <div class="col-md-4 col-sm-4 col-xs-12 wow fadeInLeft" data-wow-offset="50" data-wow-delay="0.6s">
            <div class="media">
              <div class="media-heading-wrapper">
                <div class="media-object pull-left">
                  <i class="fa fa-mobile"></i>
                </div>
                <h3 class="media-heading">FULLY RESPONSIVE</h3>
              </div>
              <div class="media-body">
                <p>Awesome responsive template is provided by <a rel="nofollow" href="http://www.templatemo.com" target="_parent">templatemo</a> website. This is Bootstrap v3.3.2 layout built on HTML5 CSS3. You can use this for any purpose. Please tell your friends about it.</p>
              </div>
            </div>
          </div>
          <div class="col-md-4 col-sm-4 col-xs-12 wow fadeInUp" data-wow-offset="50" data-wow-delay="0.9s">
            <div class="media">
              <div class="media-heading-wrapper">
                <div class="media-object pull-left">
                  <i class="fa fa-comment-o"></i>
                </div>
                <h3 class="media-heading">FREE SUPPORT</h3>
              </div>
              <div class="media-body">
                <p>Credits go to <a rel="nofollow" href="http://pixabay.com">Pixabay</a> for homepage image and <a rel="nofollow" href="http://unsplash.com">Unsplash</a> for portfolio images. Lorem ipsum dolor sit amet, consectetur adipiscing elitquisque tempus ac eget diam et laoreet phasellus ut nisi id leo molestie.</p>
              </div>
            </div>
          </div>
          <div class="col-md-4 col-sm-4 col-xs-12 wow fadeInRight" data-wow-offset="50" data-wow-delay="0.6s">
            <div class="media">
              <div class="media-heading-wrapper">
                <div class="media-object pull-left">
                  <i class="fa fa-html5"></i>
                </div>
                <h3 class="media-heading">HTML5 &AMP; CSS3</h3>
              </div>
              <div class="media-body">
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elitquisque tempus ac eget diam et laoreet phasellus ut nisi id leo molestie. Adipiscing vitae vel quam proin eget mauris eget. Lorem ipsum dolor sit amet.</p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
    <!-- end about -->

    <!-- start team -->
    <section id="team">
      <div class="container">
        <div class="row">
          <div class="col-md-12">
            <h2 class="wow bounceIn" data-wow-offset="50" data-wow-delay="0.3s"><span>AWESOME</span> TEAM</h2>
          </div>
          <div class="col-md-3 col-sm-6 col-xs-12 wow fadeIn" data-wow-offset="50" data-wow-delay="1.3s">
            <div class="team-wrapper">
              <img src="~/assets/images/team-img1.jpg" class="img-responsive" alt="team img 1">
              <div class="team-des">
                <h4>TRACY</h4>
                <span>Designer</span>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elitquisque tempus ac eget diam et laoreet phasellus ut nisi id leo molest.</p>
              </div>
            </div>
          </div>
          <div class="col-md-3 col-sm-6 col-xs-12 wow fadeIn" data-wow-offset="50" data-wow-delay="1.6s">
            <div class="team-wrapper">
              <img src="~/assets/images/team-img2.jpg" class="img-responsive" alt="team img 2">
              <div class="team-des">
                <h4>MARY</h4>
                <span>Developer</span>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elitquisque tempus ac eget diam et laoreet phasellus ut nisi id leo molest.</p>
              </div>
            </div>
          </div>
          <div class="col-md-3 col-sm-6 col-xs-12 wow fadeIn" data-wow-offset="50" data-wow-delay="1.3s">
            <div class="team-wrapper">
              <img src="~/assets/images/team-img3.jpg" class="img-responsive" alt="team img 3">
              <div class="team-des">
                <h4>JULIA</h4>
                <span>Director</span>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elitquisque tempus ac eget diam et laoreet phasellus ut nisi id leo molest.</p>
              </div>
            </div>
          </div>
          <div class="col-md-3 col-sm-6 col-xs-12 wow fadeIn" data-wow-offset="50" data-wow-delay="1.6s">
            <div class="team-wrapper">
              <img src="~/assets/images/team-img4.jpg" class="img-responsive" alt="team img 4">
              <div class="team-des">
                <h4>LINDA</h4>
                <span>Manager</span>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elitquisque tempus ac eget diam et laoreet phasellus ut nisi id leo molest.</p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
    <!-- end team -->

    <!-- start service -->
    <section id="service">
      <div class="container">
        <div class="row">
          <div class="col-md-12">
            <h2 class="wow bounceIn" data-wow-offset="50" data-wow-delay="0.3s">OUR <span>AWESOME</span> THINGS</h2>
          </div>
          <div class="col-md-4 wow fadeIn" data-wow-offset="50" data-wow-delay="0.6s">
            <i class="fa fa-laptop"></i>
            <h4>Web Design</h4>
            <p>Lorem ipsum dolor sit amet, consectetur adipiscing elitquisque tempus ac eget diam et laoreet phasellus ut nisi id leo molestie. Adipiscing vitae vel quam proin eget mauris eget. Lorem ipsum dolor sit amet, consectetur adipiscing elitquisque tempus ac eget diam et laoreet phasellus ut nisi id leo molestie.</p>
          </div>
          <div class="col-md-4 active wow fadeIn" data-wow-offset="50" data-wow-delay="0.9s">
            <i class="fa fa-cloud"></i>
            <h4>Cloud Computing</h4>
            <p>Lorem ipsum dolor sit amet, consectetur adipiscing elitquisque tempus ac eget diam et laoreet phasellus ut nisi id leo molestie. Adipiscing vitae vel quam proin eget mauris eget. Lorem ipsum dolor sit amet, consectetur adipiscing elitquisque tempus ac eget diam et laoreet phasellus ut nisi id leo molestie.</p>
          </div>
          <div class="col-md-4 wow fadeIn" data-wow-offset="50" data-wow-delay="0.6s">
            <i class="fa fa-cog"></i>
            <h4>UX Design</h4>
            <p>Lorem ipsum dolor sit amet, consectetur adipiscing elitquisque tempus ac eget diam et laoreet phasellus ut nisi id leo molestie. Adipiscing vitae vel quam proin eget mauris eget. Lorem ipsum dolor sit amet, consectetur adipiscing elitquisque tempus ac eget diam et laoreet phasellus ut nisi id leo molestie.</p>
          </div>
        </div>
      </div>
    </section>
    <!-- end servie -->

    <!-- start portfolio -->
    <section id="portfolio">
      <div class="container">
        <div class="row">
          <div class="col-md-12">
            <h2 class="wow bounceIn" data-wow-offset="50" data-wow-delay="0.3s"><span>AWESOME</span> PORTFOLIO</h2>
          </div>
          <div class="col-md-3 col-sm-6 col-xs-12 wow fadeIn" data-wow-offset="50" data-wow-delay="0.6s">
            <div class="portfolio-thumb">
              <img src="~/assets/images/portfolio-img1.jpg" class="img-responsive" alt="portfolio img 1">
              <div class="portfolio-overlay">
                <h4>Project One</h4>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elitquisque tempus ac eget dia.</p>
                <a href="#" class="btn btn-default">DETAIL</a>
              </div>
            </div>
          </div>
          <div class="col-md-3 col-sm-6 col-xs-12 wow fadeIn" data-wow-offset="50" data-wow-delay="0.6s">
            <div class="portfolio-thumb">
              <img src="~/assets/images/portfolio-img2.jpg" class="img-responsive" alt="portfolio img 2">
              <div class="portfolio-overlay">
                <h4>Project Two</h4>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elitquisque tempus ac eget dia.</p>
                <a href="#" class="btn btn-default">DETAIL</a>
              </div>
            </div>
          </div>
          <div class="col-md-3 col-sm-6 col-xs-12 wow fadeIn" data-wow-offset="50" data-wow-delay="0.6s">
            <div class="portfolio-thumb">
              <img src="~/assets/images/portfolio-img3.jpg" class="img-responsive" alt="portfolio img 3">
              <div class="portfolio-overlay">
                <h4>Project Three</h4>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elitquisque tempus ac eget dia.</p>
                <a href="#" class="btn btn-default">DETAIL</a>
              </div>
            </div>
          </div>
          <div class="col-md-3 col-sm-6 col-xs-12 wow fadeIn" data-wow-offset="50" data-wow-delay="0.6s">
            <div class="portfolio-thumb">
              <img src="~/assets/images/portfolio-img4.jpg" class="img-responsive" alt="portfolio img 4">
              <div class="portfolio-overlay">
                <h4>Project Four</h4>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elitquisque tempus ac eget dia.</p>
                <a href="#" class="btn btn-default">DETAIL</a>
              </div>
            </div>
          </div>
          <div class="col-md-3 col-sm-6 col-xs-12 wow fadeIn" data-wow-offset="50" data-wow-delay="0.6s">
            <div class="portfolio-thumb">
              <img src="~/assets/images/portfolio-img3.jpg" class="img-responsive" alt="portfolio img 3">
              <div class="portfolio-overlay">
                <h4>Project Five</h4>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elitquisque tempus ac eget dia.</p>
                <a href="#" class="btn btn-default">DETAIL</a>
              </div>
            </div>
          </div>
          <div class="col-md-3 col-sm-6 col-xs-12 wow fadeIn" data-wow-offset="50" data-wow-delay="0.6s">
            <div class="portfolio-thumb">
              <img src="~/assets/images/portfolio-img4.jpg" class="img-responsive" alt="portfolio img 4">
              <div class="portfolio-overlay">
                <h4>Project Six</h4>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elitquisque tempus ac eget dia.</p>
                <a href="#" class="btn btn-default">DETAIL</a>
              </div>
            </div>
          </div>
          <div class="col-md-3 col-sm-6 col-xs-12 wow fadeIn" data-wow-offset="50" data-wow-delay="0.6s">
            <div class="portfolio-thumb">
              <img src="~/assets/images/portfolio-img1.jpg" class="img-responsive" alt="portfolio img 1">
              <div class="portfolio-overlay">
                <h4>Project Seven</h4>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elitquisque tempus ac eget dia.</p>
                <a href="#" class="btn btn-default">DETAIL</a>
              </div>
            </div>
          </div>
          <div class="col-md-3 col-sm-6 col-xs-12 wow fadeIn" data-wow-offset="50" data-wow-delay="0.6s">
            <div class="portfolio-thumb">
              <img src="~/assets/images/portfolio-img2.jpg" class="img-responsive" alt="portfolio img 2">
              <div class="portfolio-overlay">
                <h4>Project Eight</h4>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elitquisque tempus ac eget dia.</p>
                <a href="#" class="btn btn-default">DETAIL</a>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
    <!-- end portfolio -->

    <!-- start contact -->
    <section id="contact">
      <div class="container">
        <div class="row">
          <div class="col-md-12">
            <h2 class="wow bounceIn" data-wow-offset="50" data-wow-delay="0.3s">CONTACT <span>AWESOME</span></h2>
          </div>
          <div class="col-md-6 col-sm-6 col-xs-12 wow fadeInLeft" data-wow-offset="50" data-wow-delay="0.9s">
            <form action="#" method="post">
              <label>NAME</label>
              <input name="fullname" type="text" class="form-control" id="fullname">

              <label>EMAIL</label>
              <input name="email" type="email" class="form-control" id="email">

              <label>MESSAGE</label>
              <textarea name="message" rows="4" class="form-control" id="message"></textarea>

              <input type="submit" class="form-control">
            </form>
          </div>
          <div class="col-md-6 col-sm-6 col-xs-12 wow fadeInRight" data-wow-offset="50" data-wow-delay="0.6s">
            <address>
              <p class="address-title">OUR ADDRESS</p>
              <span>Lorem ipsum dolor sit amet, consectetur adipiscing elitquisque tempus ac eget diam et laoreet phasellus ut nisi id leo molestie.</span>
              <p><i class="fa fa-phone"></i> 010-020-0340</p>
              <p><i class="fa fa-envelope-o"></i> awesome@company.com</p>
              <p><i class="fa fa-map-marker"></i> 663 New Walk Roadside, Birdeye View, GO 11020</p>
            </address>
            <ul class="social-icon">
              <li><h4>WE ARE SOCIAL</h4></li>
              <li><a href="#" class="fa fa-facebook"></a></li>
              <li><a href="#" class="fa fa-twitter"></a></li>
              <li><a href="#" class="fa fa-instagram"></a></li>
            </ul>
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
            <p class="wow bounceIn" data-wow-offset="50" data-wow-delay="0.3s">
              Copyright &copy; 2084 Company Name</p>
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
export default {
  name: "MainLayout",
  components: {ModalEducationComponent, ModalExperienceComponent, ModalSkillsComponent, ModalMeComponent}
}
</script>

<style scoped>

</style>
