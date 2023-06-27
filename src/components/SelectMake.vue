<template>
    <div class="make-wrapper">
        <div class="select-make">
            <div class="select-make-content">
                <h2>Select a Make</h2>
                <hr/>
                <div class="make-tiles">
                    <div class="make-tile" v-for="(make, index) in makeList" :key="index">
                        <span>{{ make.make }}</span>
                        <!-- <div> -->
                        <img :src="make.img" alt="">
                        <!-- </div> -->
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'SelectMake',
    props: {
    },
    data() {
        return { 
            makeList: [
                {
                    make: 'Austin Healey',
                    img: require('../assets/img/parts/tiles/austin-healey.png')
                },
                {
                    make: 'Jaguar',
                    img: require('../assets/img/parts/tiles/jaguar.png')
                },
                {
                    make: 'MG',
                    img: require('../assets/img/parts/tiles/mg.png')
                },
                {
                    make: 'Triumph',
                    img: require('../assets/img/parts/tiles/triumph.png')
                }
            ]
        }
    },
}
</script>

<style lang="less">
    .make-wrapper {
        display: flex;
        // width: 100%;
        // margin: auto;
        // max-width: 1170px;
        background: #ececec;
        padding: 16px 8px 48px 8px;
    }

    .select-make {
        margin: auto;
        max-width: 1170px;
        width: 100%
    }

    .select-make-content {
        width: 100%;
        h2 {
            margin-bottom: 8px;
        }
        hr {
            width: 100%;
            height: 1px;
            background: #5a131c;
            margin-bottom: 24px;
        }
    }

    .make-tiles {
        display: flex;
        flex-wrap: wrap;
        justify-content: center;
    }

    .make-tile {
        display: flex;
        flex-direction: column;
        margin-bottom: 24px;
        span {
            font-weight: bold;
        }
        img {
            transform: translateX(-30px)
        };
    }

    @media screen and (max-width: 1280px) {
        .make-tile {
            align-items: center;
            span {
                padding-right: 30px;
            }
        }
    }

</style>