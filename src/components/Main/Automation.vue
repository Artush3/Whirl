<template>
    <section>
        <div class="conteiner_content flex-sb">
            <div class="desc_content">
                <h1>Your everyday tasks, automated.</h1>
                <p>Whirl lets you design and streamline<br> your everyday tasks and workflows<br> in just a few clicks.</p>
                <div class="learn_content">
                    <button><a href="#">Book a demo</a></button>
                    <button class="flex">
                        <a href="#">Learn more</a>
                        <img src="C:\Users\user\Desktop\Whirl\whirl\src\img\Main\Automation\IMAGE (1).png" alt="дearn more">
                    </button>
                </div>
            </div>
            <img src="C:\Users\user\Desktop\Whirl\whirl\src\img\Main\Automation\IMAGE (2).png" alt="картина">
        </div>
    </section>
</template>

<script>
export default {
    name: "Automation"
}
</script>

<style scoped lang="scss">
@use "../../assets/variables.scss" as *;
@use "../../assets/mixins.scss" as *;
section {
    @include main(550px);

    div.desc_content {
        max-width: 525px;

        h1 {
            @include text($fraunces, $font-size:58px, $line-height:63.8px);
        }

        p {
            @include text($inter, $font-size:20px, $line-height:30px);
            margin: 30px 0;
        }

        div.learn_content {
            @include flex(center);
            button {
                &:first-of-type {
                    @include button-a(43px, 174px, #0070A0, #FFFFFF);
                    margin-right: 20px;
                }

                &:last-of-type {
                    @include button-a(43px, 110px, #FFFFFF, #0070A0);

                    a {
                        margin-right: 5px;
                    }
                }
            }
        }
    }
}
</style>