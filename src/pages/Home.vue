<script>
import Component from '../components/Homepage/ComponentRepeat.vue';
import Leading from '../components/Homepage/LeadingOrganisations.vue';
import Form from '../components/Homepage/Form.vue';
import Awards from '../components/Awards.vue';
export default{
        name:'Home',
        props:{
            store:Object
        },
        components:{
            Component,
            Leading,
            Awards,
            Form
        },
    };
</script>

<template>
     <!--Head section-->
    <div id="first-section-Home" class="py-5">
        <div class="container py-5 mb-4">
        <div class="row">
            <div class="col-6 left text-white">
                <h1 class="display-2 fw-semibold mt-5">Unlock Your Online Growth Potential</h1>
                <h3 class="fw-normal mt-5">Online marketing to secure customer retention, leads, and sales. We focus on the bigget picture</h3>
                <button type="button" class="btn btn-lg px-5 py-2 my-5 fw-semibold">Our Services <font-awesome-icon icon="fa-solid fa-arrow-right" /></button>
            </div>
            <div class="col-6 right px-5">
                <Form/>
            </div>
        </div>
    </div>
    </div>
     <!--3 section about -->
    <Component v-for="section in store.componentRepeatHome" :section="section"/>
     <!--Brand work with section-->
    <div class="container" id="brand-Work-With-Home">
        <div class="row">
            <div class="col12 text-center">
                   <h2 class="display-4 fw-semibold mt-5">Some Brands We Work With</h2>
                   <span class="fs-4">Lorem ipsum Tempora praesentium ducimus dolore.</span>
            </div>
            <div class="col-2 my-5" v-for="image in store.brandsWorkWith">
                <img :src="image" alt="brand">
            </div>
            <div class="col-12 d-flex border-top-0 shadow-b my-5" >
                <div class="col-1 p-0"><figure class="ms-auto"><img src="https://avada.website/marketing-consultant/wp-content/uploads/sites/142/2020/06/marketing-expert-cta.png"></figure></div>
            <div class="col-2 ps-2 pt-2">
                <span class="d-block fs-4 fw-semibold">Sandy Reiff</span><small>Marketing Consultant Expert</small>
            </div>
            <div class="col-6 pt-3"><span class="fs-3 fw-semibold">Drive Leads and Sales with Avada</span></div>
            <div class="col-3"><button type="button" class="btn btn-lg px-5 mt-3"><font-awesome-icon icon="fa-solid fa-phone" /> (555) 802-1234</button></div>
            </div>
        </div>
    </div>
    <!--Leading section-->
    <div class="container my-5" id="leading">
        <div class="row">
            <div class="col-12 text-center mb-5">
                <h2 class="display-4 fw-semibold">Trusted by Leading Organisations</h2>
            </div>
            <Leading v-for="col in store.leading" :col="col" :brand="store.brandsWorkWith"/>
            <div class="col-12 text-center my-5"><button type="button" class="btn btn-lg Mainbutton mt-3">Read More Case Studies</button></div>
        </div>
    </div>
    <!--Relationship section-->
    <div style="background-color: #F6F6F7;" class="py-5 mb-5">
        <div class="container py-5">
            <div class="row py-5">
                <div class="col-6 pe-5 pt-5 mb-5">
                    <h2 class="display-4 fw-semibold pe-3">We Boost Our <br>Client's Bottom Line by Optimizing Their Growth Potential.</h2>
                    <p class="fs-4 mt-4">Lorem, ipsum dolor sit amet consectetur adipisicing elit. Dolore minus voluptas omnis debitis repudiandae qui fuga?</p>
                    <button type="button" class="btn btn-lg Mainbutton mt-4">Why Work With Us</button>
                </div>
                <div class="col-6 mb-5">
                    <img src="https://avada.website/marketing-consultant/wp-content/uploads/sites/142/2020/07/we-boost-our-clients-1200x1098.jpg" alt="" width="100%" class="rounded-3">
                </div>
                <div class="col-6 pe-5 mt-5">
                    <h3 class="fs-2">We build Relationships</h3>
                    <p class="fs-4">Lorem ipsum dolor sit amet consectetur adipisicing elit. ab nobis odit vitae perspiciatis recusandae Ut!</p>
                    <h3 class="mt-5 fs-2">Proprietary Processes</h3>
                    <p class="fs-4">Lorem ipsum dolor sit amet consectetur adipisicing elit. ab nobis odit vitae perspiciatis recusandae qui</p>
                </div>
                <div class="col-6 ps-5">
                    <div class="d-flex my-5">
                        <font-awesome-icon icon="fa-solid fa-signal" class="fs-4 p-4 rounded-4 signal" />
                        <div class="ms-4">
                            <h3 class="texthover">Accountability</h3>
                            <span>Lorem ipsum dolor sit amet adipisicing elit</span>
                        </div>
                    </div>
                    <div class="d-flex my-5">
                        <font-awesome-icon icon="fa-solid fa-signal" class="fs-4 p-4 rounded-4 signal" />
                        <div class="ms-4">
                            <h3 class="texthover">Transparency</h3>
                            <span>Lorem ipsum dolor sit amet adipisicing elit</span>
                        </div>
                    </div>
                    <div class="d-flex my-5">
                        <font-awesome-icon icon="fa-solid fa-signal" class="fs-4 p-4 rounded-4 signal" />
                        <div class="ms-4">
                            <h3 class="texthover">Investment</h3>
                            <span>Lorem ipsum dolor sit amet adipisicing elit</span>
                        </div>
                    </div>
                </div>
                <Awards/>
            </div>
        </div>
    </div>

    <div class="container py-5">
        <div class="row py-5">
            <div class="col-6">
                <img src="https://avada.website/marketing-consultant/wp-content/uploads/sites/142/2020/07/large-testimonial.jpg" alt="" width="100%" class="rounded-3">
            </div>
            <div class="col-5 px-5 pt-5">
                <p class="fw-semibold fs-3 px-5 mt-5">"The team at Avada Marketing Consultant is fabulous. they hlped us unlock our potential online and offline. We have experienced year growth due to their progressive approach."</p>
                <span class="d-block fs-5 px-5 mt-5">Kate Schadler</span>
                <small class="px-5">Marketing Consultant - Abstract</small>
            </div>
        </div>
    </div>
     <!--Marketing resources-->
    <div class="py-5" style="background-color: #F6F6F7;" id="marketing-resources">
        <div class="container py-5">
            <div class="row">
                <div class="col-6 mb-5">
                    <h2 class="display-4 fw-semibold">Marketing Resources: Insider Advice on How to Increase Online Sales</h2>
                </div>
                <div class="col-6 position-relative mb-5">
                    <button class="btn btn-lg Mainbutton position-absolute top-50 end-0">Explore All Resources</button>
                </div>
                <div class="col-4 mb-5">
                    <img src="https://avada.website/marketing-consultant/wp-content/uploads/sites/142/2020/06/blog-posts-6-1200x800.jpg" alt="a" class="rounded-3">
                    <p class="fw-semibold fs-3 pe-3 mt-3">Marketing Tips And Tricks For Your Website</p>
                </div>
                <div class="col-4 mb-5">
                    <img src="https://avada.website/marketing-consultant/wp-content/uploads/sites/142/2020/06/blog-posts-5-1200x800.jpg" alt="b" class="rounded-3">
                    <p class="fw-semibold fs-3 pe-3 mt-3">How to Write Stunning Blog Post Titles</p>
                </div>
                <div class="col-4 mb-5">
                    <img src="https://avada.website/marketing-consultant/wp-content/uploads/sites/142/2020/06/blog-posts-4-1200x800.jpg" alt="c" class="rounded-3">
                    <p class="fw-semibold fs-3 pe-3 mt-3">Techniques to Reduce Facebook Ads Spend</p>
                </div>
            </div>
        </div>
    </div>
    <!--Black container-->
    <div class="py-5" style="background-color: black;">
        <div class="container py-5">
            <div class="row">
                <div class="col-6 text-white">
                    <h1 class="display-2 fw-semibold">Let's Make Things Happen</h1>
                    <p class="fw-semibold fs-3 mt-4">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Recusandae delectus numquam sequi vero modi.</p>
                    <hr class="w-25 my-5">
                    <em><p class="fw-semibold fs-5">"Lorem ipsum dolor sit amet consectetur adipisicing elit. Quis temporibus sit optio alias unde commodi veritatis delectus sed, corporis totam aut aliquid consequatur ea nobis cum. Beatae a ratione animi!"</p></em>
                    <span class="d-block fs-5 mt-5 mb-2">George Anderson</span>
                    <small>MDigitalbox CEO</small>
                </div>
                <div class="col-6 pb-5">
                    <Form class="w-75 ms-auto"/>
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped lang="scss">
</style>
