<script>
export default{
        name:'Form',
    };
</script>

<template>
    <div class="text-center bg-white px-4 py-4 rounded-4 shadow-lg">
                    <figure class="mx-auto"><img src="https://avada.website/marketing-consultant/wp-content/uploads/sites/142/2020/07/marketing-consultant-expert.jpg"></figure>
                    <span class="d-block fs-5 fw-semibold fs-3">Richard Madsen</span>
                    <span class="d-block fs-5 text-secondary mt-3">Marketing Consultant Expert</span>
                    <span class="d-block number fs-5 fw-semibold mb-4 mt-3"><font-awesome-icon icon="fa-solid fa-phone" /> (555)802-1234</span>
                    <input type="text" class="form-control fs-5 py-3 my-3" placeholder="Your Name*" aria-label="Username" aria-describedby="addon-wrapping">
                    <input type="text" class="form-control fs-5 py-3 my-3" placeholder="Your Email*" aria-label="Username" aria-describedby="addon-wrapping">
                    <input type="text" class="form-control fs-5 py-3 my-3" placeholder="Your Phone Number*" aria-label="Username" aria-describedby="addon-wrapping">
                    <button type="button" class="btn btn-lg Mainbutton w-100 my-1">Get A Callback</button>
                    <small class="my-3">By submitting my data I agree to be contacted</small>
                </div>
</template>

<style scoped lang="scss">
@use '../../assets/scss/variables.scss' as *;
    figure{
        width: 100px;
        height: 100px;
        overflow: hidden;
        border-radius: 100px;
            img{
                width: 100%;
                        height: 100%;
                object-fit: cover;
            }
        }
        input{
            &:hover{
                border-color: $mainColor;
            }
        }
        .number{
            color: $mainColor;
        }
</style>
