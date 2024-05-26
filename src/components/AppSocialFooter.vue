<script>
export default{
    data(){
        return{

        }
    },
    methods:{
    },
    mounted(){
        console.log("AppSocialFooter montato")
    }
}

</script>

<template>
    <footer class="social-footer">
        <div class="social-footer-left">
            <button>SIGN-UP NOW!</button>
        </div>
        <div class="social-footer-right">
            <p>FOLLOW US</p>
            <img src="../../src/assets/img/footer-facebook.png" alt="footer-facebook.png">
            <img src="../../src/assets/img/footer-twitter.png" alt="footer-twitter.png">
            <img src="../../src/assets/img/footer-youtube.png" alt="footer-youtube.png">
            <img src="../../src/assets/img/footer-pinterest.png" alt="footer-pinterest.png">
            <img src="../../src/assets/img/footer-periscope.png" alt="footer-periscope.png">
        </div>
    </footer>

</template>

<style scoped>
.social-footer{
    width: 100%;
    display: flex;
    justify-content: space-around;
    background-color: rgb(48, 48, 48);
    padding: 2rem;
    position: relative;
    z-index: 1;
}

.social-footer-right{
    display: flex;
    align-items: center;
    gap: 1rem;
}
p{
    color: rgb(2, 130, 249);
}

button{
    color: white;
    background-color:rgb(48, 48, 48);
    padding: 0.5rem;
    border: 1px solid rgb(2, 130, 249);
}
</style>