<script>
export default {

}
</script>
<template>
    <div>
        <main>
            <div class="container">
                <div class="row">
                    <div class="col-list">
                        <div class="container">
                            <div class="row-list">
                                <div class="col-small">

                                    <ul>
                                        <li>
                                            <h4>DC COMICS</h4>
                                        </li>
                                        <li>Carachters</li>
                                        <li>Comics</li>
                                        <li>Movies</li>
                                        <li>TV</li>
                                        <li>Games</li>
                                        <li>Video</li>
                                        <li>News</li>
                                        <li>
                                            <h4>SHOP</h4>
                                        </li>
                                        <li>Shop DC</li>
                                        <li>Shop DC Collectibles</li>
                                    </ul>
                                </div>
                                <div class="col-small">

                                    <ul>
                                        <li>
                                            <h4>DC</h4>
                                        </li>
                                        <li>Terms of use</li>
                                        <li>Privacy Policy(New)</li>
                                        <li>Ad Choices</li>
                                        <li>Advertising</li>
                                        <li>Jobs</li>
                                        <li>Subscriptions</li>
                                        <li>Talent Workshop</li>
                                        <li>CPSC Certificate</li>
                                        <li>Ratings</li>
                                        <li>Shop help</li>
                                        <li>Contact us</li>

                                    </ul>
                                </div>
                                <div class="col-small">

                                    <ul>
                                        <li>
                                            <h4>SITES</h4>
                                        </li>
                                        <li>DC</li>
                                        <li>MAD Magazine</li>
                                        <li>DC Kids</li>
                                        <li>DC Universe</li>
                                        <li>DC Power Visa</li>
                                    </ul>
                                </div>
                            </div>
                        </div>
                    </div>
                    <div class="col-back">
                        <img src="../assets/img/dc-logo-bg.png" alt="">
                    </div>
                </div>
            </div>
        </main>
    </div>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables' as*;

.row {
    display: flex;
    justify-content: space-around;
    flex-wrap: wrap;
}

.row-list {
    display: flex;
    justify-content: space-evenly;
    flex-wrap: wrap;
}


main {
    background-image: url(../assets/img/footer-bg.jpg);
    height: 500px;
}

img {
    object-fit: cover;
}

h4 {
    color: white;
    font-size: 20px;
}

li {
    list-style-type: none;
    color: grey;
    font-size: 13px;
    padding-bottom: 5px;
}

h4,
li {
    font-family: Arial, Helvetica, sans-serif;
}
</style>