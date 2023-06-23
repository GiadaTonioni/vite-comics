<script>
export default {

}
</script>
<template>
    <div>
        <footer>
            <div class="container">
                <div class="row">
                    <div class="col">
                        <button>SIGN-UP NOW!</button>
                    </div>
                    <div class="col">
                        <h4>FOLLOW US</h4>
                        <div class="loghi">
                            <img src="../assets/img/footer-facebook.png" alt="">
                            <img src="../assets/img/footer-twitter.png" alt="">
                            <img src="../assets/img/footer-youtube.png" alt="">
                            <img src="../assets/img/footer-pinterest.png" alt="">
                            <img src="../assets/img/footer-periscope.png" alt="">
                        </div>
                    </div>
                </div>
            </div>
        </footer>
    </div>
</template>
<style lang="scss" scoped>
@use '../styles/partials/variables' as*;

.row {
    display: flex;
    justify-content: space-around;
    flex-wrap: wrap;
    align-items: center;
}

footer {
    background-color: rgb(67, 65, 65);
    height: 100px;
    position: relative;
    z-index: 2;
}

button {
    background-color: transparent;
    border: 2px solid rgb(0, 128, 255);
    color: white;
    padding: 10px;
    font-weight: 500;
}

h4 {
    color: rgb(0, 128, 255);
    font-family: Arial, Helvetica, sans-serif;
    display: inline-block;
}

.loghi {
    display: inline-block;
    margin-top: 15px;
    margin-left: 20px;
}

img {
    padding: 10px;
}
</style>