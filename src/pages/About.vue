<script>
import { store } from '../store';
import Awards from '../components/Awards.vue'
export default{
        name:'About',
        props:{
            store:Object
        },
        components:{
            Awards,
        },
    };


</script>

<template>
  
  <!-- PRIMA SEZIONE: titolo, sottotitolo, foto del team -->
<div class="container main-content">
  <section class="about-section text-center">
    <h2 class="section-title">We’re a Team of Marketing Consultants, Passionate in Helping Your Business Grow</h2>
    <p class="section-subtitle">Morbi porta, velit consectetur vehicula suscipit, ligula urna lacinia lectus, sit amet semper massa nibh vitae.</p>
    <a class="btn Mainbutton btn-margin" href="/contact">Get A Consultation</a>
    <img class="col-12 img-custom" decoding="async" alt="Marketing Agency Expert" title="Marketing Agency Expert" src="https://avada.website/marketing-consultant/wp-content/uploads/sites/142/2020/07/about-team-intro-scaled.jpg" >
  </section>

  <!-- SECONDA SEZIONE: colonna a sx con opzioni e colonna dx con foto -->
  <section class="margin-top">
    <div class="row">
    <div class="col-6">
        <div>
            <h2 class="display-4 fw-semibold mt-5 mb-5">We Equip Leaders With Strategy and Vision</h2>
        <div class="accordion">
          <h5 class="content-title mb"><a class="" href="#customer-service-content">  <span class="toggle-icon">+ </span>Customer Service</a></h5>
          <div id="customer-service-content" class="content-subtitle"> Curabitur ac leo nunc. Vestibulum et mauris vel ante finibus maximus nec ut leo. Integer consectetur luctus dui id convallis. Sed pellentesque erat non eu auctor tortor, sit amet egestas purus.</div>
          <h5 class="content-title mb"><a class=""  href="#online-consultation-content">  <span class="toggle-icon">+ </span>Online Consultation</a></h5>
          <div id="online-consultation-content" class="content-subtitle">Curabitur ac leo nunc. Vestibulum et mauris vel ante finibus maximus nec ut leo. Integer consectetur luctus dui id convallis. Sed pellentesque erat non eu auctor tortor, sit amet egestas purus.</div>
          <h5 class="content-title mb"><a class=""  href="#sales-management-content">  <span class="toggle-icon"> +</span> Sales Management</a></h5>
          <div id="sales-management-content" class="content-subtitle"> Curabitur ac leo nunc. Vestibulum et mauris vel ante finibus maximus nec ut leo. Integer consectetur luctus dui id convallis. Sed pellentesque erat non eu auctor tortor, sit amet egestas purus.</div>
        </div>
      </div>
    </div>
    <div class="col-6">
        <img class="image-side" src="https://avada.website/marketing-consultant/wp-content/uploads/sites/142/2020/07/who-we-are.jpg" alt="">
    </div>
    </div>
  </section>

  <!-- TERZA SEZIONE: features e dati -->
  
    <section class="features-section row text-center mt-section">
    <div class="col-md-4 feature-item">
        <font-awesome-icon class="toggle-icon" icon="fa-solid fa-chart-simple" />
      <h4 class="feature-title ">245%</h4>
      <p class="feature-subtitle ">Successful Rate
</p>
<p class="fs-6 fw-semibold">Curabitur ac leo nunc. Vestibulum et mauris vel ante finibus.</p>
    </div>
    <div class="col-md-4 feature-item">
        <font-awesome-icon class="toggle-icon" icon="fa-solid fa-bullseye" />
      <h4 class="feature-title ">#1</h4>
      <p class="feature-subtitle ">Marketing Firm</p>
      <p class="fs-6 fw-semibold">Curabitur ac leo nunc. Vestibulum et mauris vel ante finibus.</p>
    </div>
    <div class="col-md-4 feature-item">
        <font-awesome-icon class="toggle-icon" icon="fa-solid fa-lightbulb" />
      <h4 class="feature-title ">520+</h4>
      <p class="feature-subtitle ">Business</p>
      <p class="fs-6 fw-semibold">Curabitur ac leo nunc. Vestibulum et mauris vel ante finibus.</p>
    </div>
  </section>

  

  <section class="margin-top ">
    <div class="row">
            <div class="col-6">
                <img class="image-side mb-5" src="https://avada.website/marketing-consultant/wp-content/uploads/sites/142/2020/07/we-boost-our-clients-1200x1098.jpg" alt="">
            </div>
            <div class="col-6">
     
            <h2 class="display-4 fw-semibold ms-5">We Boost Our Clients’ Bottom Line by Optimizing Their Growth Potential.</h2>
                 <div id="customer-service-content" class="content-subtitle-display ms-5"> Quisque aliquet, libero consequat elementum convallis, erat imperdiet.</div>
                 <a class="btn Mainbutton btn-margin ms-5" href="/contact">Why Work With Us</a>
           </div>
           <Awards/>
    </div>

    <h2 class="display-4 fw-semibold mt-5 mb-5">We Boost Our Clients’ Bottom Line <br> by Optimizing Their Growth <br> Potential.</h2>
    <div class="row">
            <div class="col-6">
                <img class="image-side mb-5" src="https://avada.website/marketing-consultant/wp-content/uploads/sites/142/2020/06/marketing-consulting-hero-review-1200x1382.jpg" alt="">
            </div>
            <div class="col-6">
     
            <h4 class="feature-subtitle fw-semibold ms-5">We’re A True Partner</h4>
               <p class="ms-5 fs-5 mt-4"> Curabitur ac leo nunc. Vestibulum et mauris vel ante finibus maximus nec ut leo. Integer consectetur. Maecenas maximus blandit facilisis. Nam egestas feugiat felis. Nullam et cursus neque, eget fringilla dolor. Pellentesque congue facilisis lobortis.</p>
               
                 <h4 class="feature-subtitle fw-semibold ms-5 mt-5">Proprietary Processes</h4>
               <p class="ms-5 fs-5 mt-4 mb-5"> Curabitur ac leo nunc. Vestibulum et mauris vel ante finibus maximus nec ut leo. Integer consectetur. Maecenas maximus blandit facilisis. Nam egestas feugiat felis. Nullam et cursus neque, eget fringilla dolor. Pellentesque congue facilisis lobortis.</p>
               <hr class="line ms-5">
               <h5 class="ms-5 fs-4 mt-4">Looking for more services?</h5>
                 <a class="btn Mainbutton btn-margin ms-5 mt-4" href="/contact">Why Work With Us</a>
                 
           </div> 
           <div class="col-12 text-center img-abstract"> <img src="https://avada.website/marketing-consultant/wp-content/uploads/sites/142/2020/06/abstract.png" alt="" width="100px">
            <p class="section-subtitle fw-normal text-black mt-3">“The team at Avada Marketing Consultant is fabulous. They helped us unlock our potential online and offline. We have experienced year on year growth due to their progressive approach.”
            </p>
            <img class="rounded-pill" src="https://avada.website/marketing-consultant/wp-content/uploads/sites/142/2020/07/small-testimonial.jpg" alt="" width="60px">
            <h5>Melissa Dean</h5>
            <div>Marketing Consultant Expert</div>
    </div>
    </div>
    
  </section>
</div>
<section class="orange-section text-center">
    <div class="row">
    <h2 class="section-title2 text-center">Let’s Supercharge Your Online Growth
</h2>
<div class="col-12">
    <a class="btn btn-custom-white mt-4 " href="/contact">Book A Free Consultation</a>
</div>

<div class="col-6 fs-2 mt-3">inquiries@company.com</div>
<div class="col-6 fs-2 mt-3">Call us (555) 802-1234</div>
</div>
</section>





</template>

<style scoped lang="scss">
@use '../assets/scss/variables.scss' as *;
   .main-content {
      padding: 50px 0;
    }
    .section-title {
      font-size: 84px;
      margin-bottom: 20px;
      margin-left: 12rem;
      margin-right: 12rem;
      font-weight: 20px;
  
    }

    .section-title2 {
      font-size: 74px;
      margin-bottom: 20px;

      font-weight: 20px;
      
  
    }

    .section-subtitle {
      font-size: 30px;
      margin-bottom: 30px;
      margin-left: 10rem;
      margin-right: 10rem;
      color: #343434;
    }
 
    .side-title {
      font-size: 54px;
      margin-top: 20px;
margin-left: 30px;
margin-right: 30px;
      font-weight: 20px;
      margin-bottom: 4rem;
    }

    .side-title2 {
      font-size: 54px;
      margin-top: 20px;

margin-right: 30px;
      font-weight: 20px;
      margin-bottom: 4rem;
    }

    .btn-custom {
     background-color: $mainColor;
     color: white;
      border-radius: 10px;
      padding: 0.7rem 2rem; 
      font-size: 1.1rem; 
    }
    .btn-custom:hover {
      background-color: $mainColorDarker;
      color: white;
    
    }
    .img-custom {
      border-radius: 7px;
      margin-top: 4rem;
    }

.image-side {
    width: 100%;
      height: auto;
      border-radius: 7px;
}
.img-award {
    width: 45%;
      height: auto;
   
}


.margin-top {
    margin-top: 8rem;
}
.content-title a{
    color: #030303;
  font-size: 36px;
  font-weight: normal;

  margin-left: 6rem;
margin-right: 4rem;
margin-top: 4rem;
cursor: pointer;
text-decoration: none;
}

.mb {
    margin-bottom: 3rem;
}
.content-subtitle {
  font-size: 18px;
  color: #666;
  display: none; 
  margin-left: 6rem;
margin-right: 4rem;
margin-top: 1.2rem;
margin-bottom: 2rem;


}

.toggle-icon {
  color: $mainColor;

}


.content-subtitle:target {
  display: block;

}

.content-subtitle-display{
    font-size: 28px;
  color: #020202;

  margin-left: 2rem;
margin-right: 4rem;
margin-top: 1.2rem;
margin-bottom: 2rem;
}
.feature-title {
    font-size: 70px;
    margin-top: 10px;
  
}

.feature-subtitle {
    font-size: 30px;
    margin-top: 10px;
  font-weight: normal
}

.mt-section {
    margin-top: 8rem;
}

.content-title a:hover {
    color: $mainColor ;
}

.full-width-bg {
  width: 100%;
  background-color: #f5f5f5;
  padding: 50px 0; 
}
.container-fluid {
  padding-right: 0;
  padding-left: 0;
}

.btn-margin {

      margin-left: 2rem;
}

.btn-custom2:hover {
    background-color: $mainColorDarker;
     color: white;
      border-radius: 10px;
      padding: 0.7rem 2rem; 
      font-size: 1.1rem; 
      margin-left: 2rem;
}

.btn-custom3 {
    background-color: $mainColor;
     color: white;
      border-radius: 10px;
      padding: 0.7rem 2rem; 
      font-size: 1.1rem; 
    
}
.btn-custom3:hover {
    background-color: $mainColorDarker;
     color: white;
      border-radius: 10px;
      padding: 0.7rem 2rem; 
      font-size: 1.1rem; 
    
}
.btn-custom-white{
    background-color: white;
     color: rgb(0, 0, 0);
      border-radius: 10px;
      padding: 0.7rem 2rem; 
      font-size: 1.1rem; 
      border: 2px solid black;
}
.btn-custom-white:hover{
    background-color: $mainColor;
     color: rgb(255, 255, 255);
      border-radius: 10px;
      padding: 0.7rem 2rem; 
      font-size: 1.1rem; 
      border: 2px solid rgb(255, 255, 255);
}
.img-abstract{

height: auto;
margin: 0 auto;
margin-top: 80px;
}

.orange-section {
    background-color: $mainColor; 
    color: #fff; 
    padding: 50px 0;
}

.line{

margin-right: 500px;
}
</style>
