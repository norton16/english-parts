<template>
    <div>
        <div class="footer-wrapper">
            <div class="footer-content">
                <div>
                    <h2>About</h2>
                    <ul>
                        <li>
                            <a>Accepted Payment</a>
                        </li>
                        <li>
                            <a>Contact Us</a>
                        </li>
                        <li>
                            <a>Policies</a>
                        </li>
                        <li>
                            <a>Refunds</a>
                        </li>
                        <li>
                            <a>Returns</a>
                        </li>
                    </ul>
                </div>
                <div>
                    <h2>Legal</h2>
                    <ul>
                        <li>
                            <a>Policies</a>
                        </li>
                    </ul>
                </div>
                <div>
                    <h2>Links</h2>
                    <ul>
                        <li>
                            <a>My Information</a>
                        </li>
                        <li>
                            <a>Testimonials</a>
                        </li>
                    </ul>
                </div>
            </div>
            <div class="footer-bottom">
                <hr>
                <div>
                    <img src="../assets/img/icons/default/disclaimer-white.png" alt="">
                    <span>
                        While every reasonable effort is made to ensure the accuracy of this data, we are not responsible for any errors or omissions contained on these pages. Please verify any information in question with a sales representative.
                    </span>
                </div>
            </div>
        </div>
        <div class="footer-end">
            <img src="../assets/img/logos/simplepart-logo-dark.png" alt="">
            <span>© 2021 EnglishParts.com</span>
        </div>
    </div>
</template>

<script>
export default {
    name: 'FooterBar',
}
</script>

<style lang="less">
    .footer-wrapper {
        background: #072847;
        padding: 16px 8px 48px 8px;
        color: #ffffff;
    }

    .footer-bottom {
        display: flex;
        margin: auto;
        max-width: 1170px;
        width: 100%;
        flex-direction: column;
        div {
            display: flex;
            align-items: center;
        }
        hr {
            width: 100%;
            background: #ffffff;
            height: 1px;
            margin: 16px 0px;
        }
        span {
            font-size: 10px;
        }
        img {
            width: 18px;
            height: 18px;
            margin-right: 8px;
        }
    }

    .footer-end {
        display: flex;
        margin: auto;
        max-width: 1170px;
        width: 100%;
        font-size: 10px;
        justify-content: space-between;
        padding: 24px 8px;
        img {
            height: 12px;
            width: max-content;
        }
    }

    .footer-content {
        display: flex;
        margin: auto;
        max-width: 1170px;
        width: 100%;
        div {
            flex: 0 0 24%; 
        }
        h2 {
            font-size: 14px;
            text-transform: uppercase;
            margin: 4px 0px;
        }
        ul {
            list-style-type: none;
            padding: 0;
            margin: 4px 0px;
        }
        li {
            font-size: 12px;
            padding-bottom: 4px;
        }
        a:hover {
            text-decoration: underline;
            cursor: pointer;
        }
    }

    @media screen and (max-width: 1024px) {
        .footer-content {
            flex-direction: column;
        }
    }

    @media screen and (max-width: 768px) {
        .footer-end {
            flex-direction: column-reverse;
            img {
                margin-top: 16px;
            }
        }
    }
</style>