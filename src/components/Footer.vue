<template>
    <footer>
        <div class="conteiner_content">
            <div class="nav_content_footer">
                <div class="builder">
                    <img src="..\img\Header\IMAGE.png" alt="фото">
                    <p>Built by <span>Nikolai Bain</span>.</p>
                    <p>Powered by <span>Webflow</span>.</p>
                </div>
                <div class="desccription">
                    <div class="desc">
                        <h3>Info</h3>
                        <p>Features</p>
                        <p>Pricing</p>
                        <p>Blog</p>
                        <p>Support</p>
                        <p>Terms & Conditions</p>
                        <p>Privacy Policy</p>
                    </div>
                    <div class="desc">
                        <h3>Admin</h3>
                        <p>Style Guide</p>
                        <p>Licenses</p>
                        <p>Instructions</p>
                        <p>Changelog</p>
                        <p>Password</p>
                        <p>404</p>
                    </div>
                    <div class="desc">
                        <h3>Newsletter</h3>
                        <h2>Sign up for the latest news, company insights, and Whirl updates.</h2>
                        <div class="input_content">
                            <input type="text" placeholder="Your email">
                            <img src="..\img\Automation\IMAGE (1).png" alt="">
                        </div>
                    </div>
                </div>
            </div>
            <hr class="hr-line">
            <div class="nav">
                <p>© 2022 Whirl. All Rights Reserved. Illustrations by <span>Streamline</span>.</p>
                <div class="vav_social">
                    <img src="..\img\Footer\Frame (1).png" alt="фото">
                    <img src="..\img\Footer\Frame (2).png" alt="фото">
                    <img src="..\img\Footer\Frame (3).png" alt="фото">
                </div>
            </div>
        </div>
    </footer>
</template>

<script>
export default {
    name: "Footer"
}
</script>

<style scoped lang="scss">
@use "../assets/mixins.scss" as *;
@use "../assets/variables.scss" as *;
footer {
    @include main(400px);

    div.nav_content_footer {
        @include flex(start, space-between);

        div.builder {
            p {
                &:first-of-type {
                    margin-top: 15px;
                }
                @include text($inter, $font-size:14px, $line-height:19.6px);
                span {
                    color: #0070A0;
                }
            }
        }

        div.desccription {
            width: 660px;
            @include flex(start, space-between);

            div.desc {
                width: 216px;

                h3 {
                    @include text($inter, $font-size:15px, $line-height:24px);
                }

                > p {
                    margin-top: 10px;
                    @include text($inter, $font-size:14px, $line-height:20px, $color:#626A72);
                }

                h2 {
                    margin: 10px 0;
                    @include text($inter, $line-height:24px);
                }

                div.input_content {
                    @include flex(center);
                    input {
                        border-bottom: 1px solid silver;
                        height: 44px;
                        padding-left: 10px;
                        @include text($inter, $font-size:13px, $color:#626A72);
                    }
                }
            }
        }
    }

    .hr-line {
        margin: 50px 0;
        border-top: 1px solid #DEE5EB;
    }

    div.nav {
        @include flex(center, space-between);

        p {
            @include text($inter, $font-size:13px);

            span {
                color: #0070A0;
            }
        }

        div.vav_social {
            img {
                &:not(:first-of-type) {
                    margin-left: 20px;
                }
            }
        }
    }
}
</style>