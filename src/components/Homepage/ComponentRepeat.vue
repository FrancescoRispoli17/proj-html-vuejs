<script>
export default{
        name:'Footer',
        props:{
            section:Object
        },
        methods:{
            getimage(img){
            return new URL(img,import.meta.url).href
            },
        }
    };
</script>

<template>
    <div class="container">
        <div class="row">
            <div class="col-7 flex-shrink" v-show="section.id!==1" :class="{position3section:section.id==2}">
                    <img v-for="(image,index) in section.images" class="position-absolute" :src="getimage(image)" style="width: 500px;">
            </div>
            <div class="col-5 py-5">
                <div id="aaa" class="rounded-circle text-white fs-5 text-center pt-1" 
                    :class="{'bg-primary':section.logoText.id==0, 'bg-warning':section.logoText.id==1, green:section.logoText.id==2}">
                     <font-awesome-icon icon="fa-brands fa-squarespace" style="margin-top: 5px;"/> 
                </div>
                <span class="fw-semibold fs-4 ms-3">{{ section.logoText.text }}</span>
                <h2 class="display-4 fw-semibold mt-3">{{ section.title }}</h2>
                <p class="fs-4">{{ section.text }}</p>
                <button type="button" class="btn btn-lg Mainbutton mt-3">{{section.button}}</button>
            </div>
            <div class="col-7 flex-shrink" v-show="section.id===1">
                <img v-for="(image,index) in section.images" class="position-absolute" :src="getimage(image)" :class="{position4:index==0,position5:index==1,position6:index==2,position7:index==3}" >
            </div>
        </div>
    </div>
</template>

<style scoped lang="scss">
@use '../../assets/scss/variables.scss' as *;
.green{
    background-color: rgb(35, 212, 44);
}
.container{
    margin-top:10rem;
    .position3section{
            img{
                &:first-child{
                    left: 140px;
                    width: 370px !important;
                }
                &:nth-child(2){
                    top: 120px;
                    left: 223px;
                    width: 330px !important;
                }
                &:nth-child(3){
                    top: 310px;
                    left: 290px;
                    width: 200px !important;
                }
                &:nth-child(4){
                    top: 100px;
                    left: 200px;
                    width: 320px !important;
                }
                &:nth-child(5){
                    top: 45px;
                    width: 330px !important;
                }
            }
        }
    .col-7{
        position: relative;
        .position4{
            top: -20px;
            width: 650px;
        }
        .position5{
            top: 70px;
            left: 150px;
            width: 300px;
        }
        .position6{
            top: 170px;
            left: 310px;
            width: 300px;
        }
        .position7{
            top: 130px;
            left: 540px;
            width: 100px;
        }
    }
    div .rounded-circle{
        width: 40px;
        height: 40px;
        display: inline-block;
    }
}

</style>
