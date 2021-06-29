<template>
  <div>
    <b-button @click="show=true" class="modal_btn">Experience</b-button>

    <b-modal
      v-model="show"
      title="Experience"
      size="xl"
      :hide-footer=true
      modal-class="modal_backdrop"
    >
      <b-container fluid>
        <div class="about">
          <div class="row">
            <div class="col-md-4 about-left ">
              <img src="~/assets/images/team-img1.jpg" class="img-fluid" alt="asraf porag">
            </div>
            <div class="col-md-8 about-right">
              <h3>Hi, i'm <span>S. Asraf Porag </span></h3>
              <h4>Full Stack Developer </h4>
              <ul class="address">
                <li>
                  <ul class="agileits-address-text ">
                    <li><b>D.O.B</b></li>
                    <li>14-10-1988</li>
                  </ul>
                </li>
                <li>
                  <ul class="agileits-address-text">
                    <li><b>PHONE </b></li>
                    <li>+880 1828 96 32 35</li>
                  </ul>
                </li>
                <li>
                  <ul class="agileits-address-text">
                    <li><b>ADDRESS </b></li>
                    <li>Gazipur City, Dhaka, Bangladesh.</li>
                  </ul>
                </li>
                <li>
                  <ul class="agileits-address-text">
                    <li><b>E-MAIL </b></li>
                    <li><a href="mailto:smauhp@gmail.com"> smauhp@gmail.com</a></li>
                  </ul>
                </li>
                <li>
                  <ul class="agileits-address-text">
                    <li><b>WEBSITE </b></li>
                    <li><a href="https://asrafporag.netlify.app" target="_blank">asrafporag.netlify.app</a></li>
                  </ul>
                </li>
              </ul>
            </div>
          </div>
          <div class="row">
            <div class="col-md-12">
              <div class="about-text">
                <p>I’m a Full Stack Developer with experience in designing, developing, and implementing applications and solutions using a range of technologies and programming languages like Php, Java, JavaScript. </p>
                <p class="agile-br">I’m also very skilled in front-end languages like HTML, CSS. Seeking to leverage broad development experience and hands-on technical expertise in a challenging role as a Full-stack Developer.</p>
              </div>
            </div>
          </div>
        </div>
      </b-container>
    </b-modal>
  </div>
</template>

<script>
export default {
  name: "ModalExperienceComponent",
  data() {
    return {
      show: false,
    }
  }
}
</script>

<style scoped>
.modal_btn{
  padding-top: 16px;
  padding-bottom: 16px;
  background-color: rgba(59,187,181,1);
  border: 0;
  border-radius: 0;
  text-transform: capitalize;
  color: #303030 !important;
  transition: 0.5s background linear;
}
.modal_btn:hover{
  background-color: rgba(143,145,152,1);
  transition: 0.5s background linear;
}
.modal_btn:hover{
  transition: 0.5s color linear;
  color: #ffffff !important;
}
/deep/ .modal_backdrop {
  background: #11a8cf !important;
}
/deep/ .modal-content {
  background: url("../assets/images/modal-bg.png") #000 repeat;
}
/deep/ .modal-header {
  padding-top: 30px !important;
  border-bottom: 0;
}
/deep/ .modal-title{
  color: #ffffff;
  padding-left: 20px;
}
/deep/ .modal-header .close{
  color: #ffffff;
  padding-right: 20px;
}
/deep/ .modal-body {
  padding-right: 15px !important;
  padding-left: 15px !important;
  padding-top: 35px;
  padding-bottom: 35px;
}

</style>

