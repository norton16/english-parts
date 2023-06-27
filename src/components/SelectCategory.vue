<template>
    <div class="select-category">
        <div class="select-category-content">
            <h2>Select a Category</h2>
            <hr/>
            <div class="category-tiles">
                    <div class="category-tile" v-for="(category, index) in categories" :key="index">
                        <span class="category-name">{{ category.name }}</span>
                        <div class="category-tile-bottom">
                            <span class="category-see">See more</span>
                            <img :src="category.img" alt="">
                        </div>
                    </div>
                </div>
        </div>
    </div>
</template>

<script>
// import json from "../assets/json/categories.json";
export default {
    name: 'SelectCategory',
    data() {
        return {
            categories: [
                {
                    name: "Body",
                    img: require('../assets/img/parts/tiles/body.jpg')
                },
                {
                    name: "Brake System",
                    img: require('../assets/img/parts/tiles/brake-system.jpg')
                },
                {
                    name: "Cables",
                    img: require('../assets/img/parts/tiles/cables.jpg')
                },
                {
                    name: "Car Care, Tools and Shop Supplies",
                    img: require('../assets/img/parts/tiles/car-care.jpg')
                },
                {
                    name: "Competition Parts",
                    img: require('../assets/img/parts/tiles/competition-parts.jpg')
                },
                {
                    name: "Convertible Tops, Hard Tops and Tonneau Covers",
                    img: require('../assets/img/parts/tiles/tops-covers.jpg')
                },
                {
                    name: "Cooling System",
                    img: require('../assets/img/parts/tiles/cooling.jpg')
                },
                {
                    name: "Electrical Components",
                    img: require('../assets/img/parts/tiles/electrical-components.jpg')
                },
                {
                    name: "Engine and Driveline",
                    img: require('../assets/img/parts/tiles/engine-driveline.jpg')
                },
                {
                    name: "Exhaust and Emissions",
                    img: require('../assets/img/parts/tiles/exhaust-emission.jpg')
                },
                {
                    name: "Exterior",
                    img: require('../assets/img/parts/tiles/exterior.jpg')
                },
                {
                    name: "Fuel Systems",
                    img: require('../assets/img/parts/tiles/fuel-system.jpg')
                },
                {
                    name: "Interior",
                    img: require('../assets/img/parts/tiles/interior.jpg')
                },
                {
                    name: "Maintenance",
                    img: require('../assets/img/parts/tiles/maintenance.jpg')
                },
                {
                    name: "Oil System",
                    img: require('../assets/img/parts/tiles/oil-system.jpg')
                },
                {
                    name: "Performance & Handling",
                    img: require('../assets/img/parts/tiles/performance-handling.jpg')
                },
                {
                    name: "Suspension",
                    img: require('../assets/img/parts/tiles/suspension.jpg')
                },
                {
                    name: "Transmission, Gearbox and Clutch",
                    img: require('../assets/img/parts/tiles/transmission.jpg')
                },
            ]
    }
    }
}
</script>

<style lang="less">
    .select-category {
        margin: auto;
        max-width: 1170px;
        width: 100%;
        padding: 16px 8px 48px 8px;
    }

    .select-category-content {
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
    
    .category-tiles {
        display: flex;
        flex-wrap: wrap;
    }

    .category-tile {
        display: flex;
        flex-direction: column;
        justify-content: space-between;
        border: 1px solid #f4f3f3;
        flex: 0 0 20%; 
        padding: 12px;
        margin: 0px 16px 16px 0px;
        .category-name {
            font-weight: bold;
            display: inline-block;
            max-width: 60%;
        }
        .category-see {
            font-size: 10px;
        }
    }
    
    .category-tile:hover {
        border-color: black;
        text-decoration: underline;
        cursor: pointer;
    }

    .category-tile-bottom {
        display: flex;
        justify-content: space-between;
        align-items: baseline;
        img {
            width: 77px;
        }
    }

    @media screen and (max-width: 480px) {
        .category-tile {
            width: 100%;
            flex: auto;
        }
        .select-category-content {
            max-width: 100% !important;
        }
    }

    @media screen and (max-width: 1280px) {
        .select-category-content {
            max-width: 80%;
            margin: auto;
        }
    }
</style>