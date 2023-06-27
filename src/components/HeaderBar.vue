<template>
    <div class="header">
        <span class="alert">       
            Browse our complete catalog of OEM and licensed British heritage parts for your 
            classic British automobile. | Kalamazoo, MI
        </span>
        <div class="header-about">
            <img class="header-logo" alt="logo" src="../assets/img/logos/logo.png">
            <div class="header-about-right">
                <div class="mobile-menu">
                    <div class="menu-bar"></div>
                    <div class="menu-bar"></div>
                    <div class="menu-bar"></div>
                </div>
                <div class="header-about-right-top">
                    <h1>EnglishParts.com</h1>
                    <ul class="header-menu">
                        <li>
                            <a>Parts</a>
                            <img src="../assets/img/icons/default/arrow-down.png" alt="">
                        </li>
                        <li>
                            <a>About Us</a>
                            <img class="arrow-right" src="../assets/img/icons/default/arrow-down.png" alt="">
                        </li>
                    </ul>
                </div>
                <div class="header-contact">
                    <div>
                        <img src="../assets/img/icons/default/header-location.png" alt="">
                        <span>5850 Stadium Dr, Kalamazoo, MI 49009</span>
                    </div>
                    <div>
                        <img src="../assets/img/icons/default/header-phone.png" alt="">
                        <a href="tel:+8664671776">866.467.1776</a>
                    </div>
                    <div>
                        <img src="../assets/img/icons/default/header-email.png" alt="">
                        <a href="mailto:sales@englishparts.com">sales@englishparts.com</a>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'HeaderBar',
    props: {
    }
}
</script>

<style scoped lang="less">
    .header {
        display: flex;
        flex-direction: column;
        max-width: 1170px;
        margin: auto;
        margin-bottom: 16px;
        padding: 0px 8px;
        .alert {
            color: #16171a ;
            font-weight: bold;
            font-size: 12px;
        }
    }

    .header-about {
        display: flex;
        margin-top: 16px;
        .header-logo {
            width: 54px;
            height: 54px;
            padding: 0px 32px;
        }
        h1 {
            font-weight: bold;
            font-size: 22px;
            margin: 0px;
        }
    }

    .header-about-right {
        width: 100%;
        display: flex;
        flex-direction: column;
        justify-content: space-between;
        .header-about-right-top {
            display: flex;
            justify-content: space-between;
            align-items: baseline;
        }
        .header-menu {
            text-decoration: none;
            list-style: none;
            display: flex;
            margin: 0px;
            font-weight: bold;
            font-size: 14px;
            img {
                width: 10px;
                padding-left: 8px;
            }
            .arrow-right {
                transform: rotate(-90deg);
            }
            li:nth-of-type(1) {
                margin-right: 16px;
            }   
        }
    }

    .header-contact {
        display: flex;
        font-size: 12px;
        font-weight: initial !important;
        img {
            height: 12px;
            margin-right: 2px;
        }
        div {
            display: flex;
            align-items: center;
            margin-right: 8px;
        }
        a {
            text-decoration: none;
            color: initial;
        }
    }

    .mobile-menu {
        border-radius: 4px;
        border: 1px solid lightgray;
        padding: 4px 8px 8px 8px;
        .menu-bar {
            height: 2px;
            margin-top: 4px;
            width: 22px;
            background: #888888;
        }
    }

    .mobile-menu:hover {
        background: #dddddd;
        cursor: pointer;
    }

    @media screen and (max-width: 768px) {
        .header-about {
            padding-left: 0px;
            h1 {
                font-size: 18px;
            }
        }
        .header-about-right {
            flex-direction: row-reverse;
            align-items: center;
        }
        .header-logo {
            width: 40px !important;
            height: 40px !important;
            padding-left: 0px !important;
        }
        .header-menu, .header-contact {
            display: none !important;
        }
    }
    
    @media screen and (min-width: 768px) {
        .mobile-menu {
            display: none;
        }
    }
</style>