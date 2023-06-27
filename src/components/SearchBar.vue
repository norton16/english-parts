<template>
    <div class="search-bar">
        <div class="search-bar-container">
            <div class="search-bar-left search-box">
                <img class="search-box-small" src="../assets/img/icons/default/utilitybar-search.png" alt="">
                <input class="word-search" type="text" placeholder="Search by Keywords, Part Numbers or BIN">
                <div class="submit-btn search-box-small">
                    GO
                </div>
            </div>
            <div class="search-bar-right">
                <div class="search-box dropdown">
                    <div>
                        <span>Select Your Vehicle</span>
                    </div>
                    <div class="submit-btn search-box-small">
                        <img class="search-box-small" src="../assets/img/icons/default/utilitybar-arrow.png" alt="">
                    </div>
                </div>
                <div class="cart">
                    <img class="search-box-small" src="../assets/img/icons/default/cart-full.png" alt="">
                    <span>0</span>
                </div>
            </div>
        </div>
    </div>
    <div class="hero-welcome">
        <a href="">Welcome to EnglishParts.com, your home for Jaguar, MG, Triumph and Austin Healey Parts!</a>
    </div>
</template>

<script>
export default {
    name: 'SearchBar',
    props: {
    }
}
</script>

<style lang="less">
    @border-color:#ececec;
    @dark-red: #9e1e23;
    @white: #ffffff;
    @black: #000000;

    .search-bar {
        border: 1px solid @border-color;
        background: #fafafa;
        padding: 12px 24px;
    }

    .search-bar-container {
        display: flex;
        width: 100%;
        margin: auto;
        max-width: 1170px;
    }

    .search-bar-right {
        display: flex;
        width: 30%;
    }
    
    .search-box {
        width: 70%;
        display: flex;
        align-items: center;
        border: 1px solid @border-color;
        background: @white;
        margin-right: 8px;
        max-height: 40px;
        .submit-btn {
            margin-left: auto;
        }
        .submit-btn:hover {
            background: #e6e6e6;
            cursor: pointer;
        }
        .search-box-small {
            padding: 8px;
            color: #9e1e23;
            font-weight: bold;
            font-size: 12px;
        }
        .word-search {
            border: none;
            font-weight: bold;
            color: #555555;
            width: 100%;
            height: 40px;
            border: 1px solid @border-color;
            border-left: none;
        }
        .word-search:focus {
            text-decoration: underline;
            color: #000000;
        }
        img {
            width: 18px;
        }
    }

    .dropdown {
        display: flex;
        width: 85%;
        font-size: 12px;
        padding-left: 8px;
        font-weight: bold;
        .submit-btn {
            display: flex;
            border-left: 1px solid @border-color;
        }
    }

    .cart {
        display: flex;
        align-items: center;
        justify-content: space-evenly;
        background: @dark-red;
        padding: 6px;
        width: 15%;
        max-height: 40px;
        img {
            height: 18px;
        }
        span {
            color: @white;
            font-size: 24px;
        }
    }

    .hero-welcome {
        max-width: 1170px;
        margin: auto;
        padding: 8px;
        max-width: 1170px;
        a {
            font-size: 12px;
            text-decoration: none;
            color: @black;
        }
    }

    @media screen and (max-width: 768px) {
        .search-bar {
            padding: 8px;
        }
        .search-bar-container {
            flex-direction: column;
            .search-bar-left, .search-bar-right {
                width: 100%;
            }
            .search-bar-left {
                margin-bottom: 8px;
            }
        }
    }
</style>