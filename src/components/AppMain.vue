<script>
export default {
    data() {
        return {
            comics: [
                {
                    "thumb": "https://www.coverbrowser.com/image/action-comics/1-1.jpg",
                    "price": "$19.99",
                    "series": "Action Comics",
                    "type": "comic book",
                },
                {
                    "thumb": "https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/M/1/M1BLLA015ISBN_0.jpg",
                    "price": "$3.99",
                    "series": "American Vampire 1976",
                    "type": "comic book",
                },
                {
                    "thumb": "https://media.wired.com/photos/593384dad80dd005b42b2817/master/w_2560%2Cc_limit/Aquaman-16.jpg",
                    "price": "$16.99",
                    "series": "Aquaman",
                    "type": "graphic novel",
                },
                {
                    "thumb": "https://d29xot63vimef3.cloudfront.net/image/batgirl/1-1.jpg",
                    "price": "$2.99",
                    "series": "Batgirl",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.posters.cz/image/750/locandine-film-in-plexiglass-batman-prowl-comic-cover-i69653.jpg",
                    "price": "$3.99",
                    "series": "Batman",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/5/50/Batman_Beyond_v.1_1.jpg",
                    "price": "$2.99",
                    "series": "Batman Beyond",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/0/0d/Batman_Superman_Vol_1_1.jpg",
                    "price": "$3.99",
                    "series": "Batman/Superman",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/c/cf/Batman_Superman_Annual_Vol_2_1.jpg",
                    "price": "$4.99",
                    "series": "Batman/Superman Annual",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/5/54/Batman_The_Joker_War_Zone_Vol_1_1.jpg",
                    "price": "$5.99",
                    "series": "Batman: The Joker War Zone",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/6/64/Batman_Three_Jokers_Collected.jpg",
                    "price": "$6.99",
                    "series": "Batman: Three Jokers",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/f/f8/Batman_White_Knight_Presents_Harley_Quinn_Vol_1_1.jpg",
                    "price": "$4.99",
                    "series": "Batman: White Knight Presents: Harley Quinn",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/c/c8/Catwoman_Vol_2_1.jpg",
                    "price": "$16.99",
                    "series": "Catwoman",
                    "type": "graphic novel",
                },
            ]
        }
    }
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

                </div>
            </div>
            <section>
                <div class="container-comics">
                    <div class="row-comics">

                        <div class="col">
                            <div class="card" v-for="(comic, index) in comics" :key="index">
                                <img :src="comic.thumb">
                                <h5>{{ comic.series }}</h5>
                                <p>{{ comic.type }}</p>
                                <p>{{ comic.price }}</p>
                            </div>
                        </div>
                    </div>
                </div>
            </section>
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
    height: 470px;
}

img {
    object-fit: cover;
    position: relative;
    z-index: 1;
    width: 50%;
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