<script>
export default {
    name: "About"
} 
</script> 

<template>
    <main>
        <div>
            <!-- HEADER SECTION -->
            <section class="header-title">
                <h1>About Page</h1>
            </section>
            <!-- JUMBOTRON -->
            <section class="about-jumbo">

                <div class="container-img">
                    <div class="overlay"></div>

                    <img src="../assets/woman-photographer-drinking-coffee-and-working-PJNBP6U-858x632.jpg"
                        alt="Profile of attractive charming curly young woman photographer drinking coffee and working with laptop on workplace">
                </div>

                <div class="container-info">
                    <!-- TITLE -->
                    <div class="title">
                        <div class="title-1">
                            <h3><span>We are a creative</span></h3>
                        </div>
                        <div class="title-2">
                            <h3><span>web </span>
                                <span class="txt-color">design agency</span>
                            </h3>
                        </div>
                    </div>
                    <!-- DIVIDER -->
                    <div class="container-bar">
                        <div class="bar">
                            <img src="/divider.svg" alt="divider">
                        </div>
                    </div>
                    <!-- PARAGRAPH -->
                    <div class="container-paragraf">
                        <p class="paragraf">
                            Far far away, behind the word mountains, far from the countries Vokalia and Consonantia, there
                            live the blind texts. Separated they live in Bookmarksgrove right at the coast of the Semantics,
                            a large language ocean.Separated they live in Bookmarksgrove.
                        </p>
                    </div>

                    <div class="container-button">
                        <div>
                            <button class="button">
                                <span>READ MORE</span>
                            </button>
                        </div>
                    </div>

                </div>
            </section>
            <!-- VISIONS SECTIONS -->
            <section class="about-visions">
                <div class="overlay-visions"></div>
                <div class="container-visions">
                    <!-- TITLE -->
                    <div class="vision-title">
                        <h3 class="title">Our Visions</h3>
                    </div>
                    <!-- DIVIDER -->
                    <div class="vision-divider">
                        <div class="container-bar">
                            <div class="bar">
                                <img src="/divider-white.svg" alt="divider">
                            </div>
                        </div>
                    </div>
                    <!-- CARDS -->
                    <div class="vision-cards">
                        <div class="overlay">

                        </div>
                    </div>
                </div>

            </section>
        </div>



    </main>
</template> 

<style lang="scss" scoped>
@use "../styles/general.scss";

main {


    // GENERAL
    .txt-color {
        color: rgb(0, 217, 166);
    }



    .header-title {
        padding: 50px 35px;
        text-align: center;
        background-color: rgb(249 249 249);

        h1 {
            font-size: 43px;
            font-weight: bold;
            color: rgb(0, 217, 166);
        }
    }

    .about-jumbo {
        margin-top: 85px;
        padding: 10% 5%;
        background-color: rgb(249 249 249);

        .container-img {
            position: relative;
            overflow: hidden;
            width: 100%;

            img {
                width: 100%;
                z-index: 1;
            }

            .overlay {
                position: absolute;
                top: 0;
                left: 0;
                width: 100%;
                height: 100%;
                background-color: rgb(249 249 249);
                z-index: 2;
                animation: slideIn 0.5s ease-out 0.3s forwards;


            }
        }

        .container-info {
            .title {
                text-align: center;
                margin-bottom: 20px;

                h3 {
                    font-size: 33px;
                    line-height: 45px;
                    font-weight: 600;
                }

                .title-1 {
                    margin: 80px 0 0;

                }

                .title-2 {
                    margin-top: 1em;

                }

            }

            .container-bar {
                display: flex;

                .bar {
                    margin: 0 auto;

                    img {
                        height: 5px;
                    }
                }
            }

            .container-paragraf {
                margin: 42px 0 0;

                .paragraf {
                    text-align: center;
                    margin: 0 0 1em;
                }
            }

            .container-button {
                margin: 80px 0 0;
                padding: 10px;

                div {
                    display: flex;
                    justify-content: center;
                    height: 100px;
                    width: 100%;
                }
            }
        }

        // ANIMATIONS
        @keyframes slideIn {
            to {
                left: 100%;
                background-color: rgb(249 249 249);
            }
        }
    }

    .about-visions {
        position: relative;
        background-image: url(../assets/interior-PTCVAAC@2x.jpg);
        background-position: center;
        background-size: cover;
        margin-top: 150px;
        margin-bottom: 0;
        padding: 142px 0 167px;
        min-height: 1000px;

        .overlay-visions {
            background-image: linear-gradient(24deg, #1cd595, #8ddc63);
            opacity: .96;
            height: 100%;
            width: 100%;
            top: 0;
            left: 0;
            position: absolute;
        }

        .vision-title {
            margin-bottom: 20px;
            position: absolute;
            width: 100%;

            .title {
                font-size: 45px;
                font-weight: 600;
                line-height: 63px;
                color: white;
                text-align: center;
            }
        }

        .vision-divider {
            position: absolute;
            width: 100%;
            top: 220px;

            .container-bar {
                display: flex;

                .bar {
                    margin: 0 auto;

                    img {
                        height: 5px;
                        fill: white;
                    }
                }
            }
        }


    }


}
</style>