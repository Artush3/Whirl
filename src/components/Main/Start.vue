<template>
    <section>
        <div class="conteiner_content">
            <div class="vontent">
                <h1>Get started with Whirl</h1>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit,<br> sed do eiusmod tempor incididunt.</p>
                <button><a href="#">Book a demo</a></button>
                <div class="conditions">
                    <div class="conditions_content">
                        <img src="..\..\img\Main\Start\Vector (1).png" alt="">
                        <p>Free 30-day trial</p>
                    </div>
                    <div class="conditions_content">
                        <img src="..\..\img\Main\Start\Vector (1).png" alt="">
                        <p>No credit-card required</p>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: "Start"
}
</script>

<style scoped lang="scss">
@use "../../assets/mixins.scss" as *;
@use "../../assets/variables.scss" as *;
section {
    @include main(550px);

    div.vontent {
        background-color: #E6F7FF;
        min-height: 370px;
        padding: 70px;

        h1 {
            @include text($fraunces, $font-size:42px);
            margin-bottom: 20px;
        }

        > p {
            @include text($inter, $font-size:18px, $line-height:27px);
        }

        button {
            margin: 25px 0;
            @include button-a(43px, 174px, #0070A0, #FFFFFF);
        }

        div.conditions {
            @include flex(center);

            div.conditions_content {
                &:first-of-type {
                    margin-right: 40px;
                }
                @include flex(center);

                p {
                    margin-left: 3px;
                    @include text($inter, $font-size:13px, $color:#626A72);
                }
            }
        }
    }
}
</style>