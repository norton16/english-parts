<template>
    <div class="hero-wrapper">
        <div class="hero">
            <div class="hero-text">
                <h2>
                    Premium Austin Healey, Jaguar, MG, and Triumph Parts 
                </h2>
                <p>Unmistakable style. That's what you love about your Austin Healey, Jaguar, MG, or Triumph. At EnglishParts.com, 
                    we carry a large selection of premium repair, maintenance and restoration parts for classic British cars. 
                    You know you can count on us because we're located in Kalamazoo, MI. Finding the right premium repair parts has always been our first priority. 
                    Our state of the art premium parts diagrams ensure that you're getting the perfect part the first time. 
                    Our experienced team knows these cars inside and out, and is here to help. Excellence. The first time, every time. </p>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'HeroSection',
    props: {
    }
}
</script>

<style lang="less">
    .hero-wrapper {
        display: flex;
    }

    .hero {
        width: 100%;
        height: 260px;
        background-image: url('../assets/img/parts/heroes/default.jpg');
    }

    .hero-text {
        background: #072847;
        color: white;
        width: 975px;
        height: 260px;
        display: flex;
        flex-direction: column;
        margin-left: auto;
        h2, p {
            width: 70%;
            padding-left: 16px;
        }
        h2 {
            margin-bottom: 12px;
        }
        p {
            font-size: 14px;
            margin-top: 0px;
        }
    }

    @media screen and (max-width: 1536px) {
        .hero {
            background-position-x: -350px;
        }
    }

    @media screen and (max-width: 1280px) {
        .hero-text {
            h2, p {
                padding: 8px 16px;
            }
        }
    }

    @media screen and (max-width: 768px) {
        .hero {
            height: auto;
            background-image: none;
        }
        .hero-text {
            height: auto;
            width: 100%;
            padding-bottom: 16px;
            h2, p {
                width: auto;
            }
        }
    }

    @media screen and (max-width: 640px) {
        .hero-text {
            width: 100%;
            span {
                padding-right: 30px;
            }
        }
    }
</style>