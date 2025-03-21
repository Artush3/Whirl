<template>
    <section>
        <div class="conteiner_content">
            <div class="desc">
                <h1>Your tasks, automated.</h1>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</p>
            </div>
            <div class="advanteges">
                <div class="content_advanteges">
                    <img src="..\..\img\Main\Automated\Снимок экрана 2022-07-25 в 00.05 1.png" alt="фото">
                    <h2>Learn your options.</h2>
                    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor.</p>
                </div>
                <div class="content_advanteges">
                    <img src="..\..\img\Main\Automated\IMAGE (14).png" alt="фото">
                    <h2>Stay informed.</h2>
                    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et doloretro.</p>
                </div>
                <div class="content_advanteges">
                    <img src="..\..\img\Main\Automated\Снимок экрана 2022-07-25 в 00.06 1.png" alt="фото">
                    <h2>Automate it all.</h2>
                    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor ipsum.</p>
                </div>
                <div class="content_advanteges">
                    <img src="..\..\img\Main\Automated\Снимок экрана 2022-07-25 в 00.06 2.png" alt="фото">
                    <h2>Stay informed.</h2>
                    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod incididunt ut labore et consectetur.</p>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: "Automated"
}
</script>

<style scoped lang="scss">
@use "../../assets/mixins.scss" as *;
@use "../../assets/variables.scss" as *;
section {
    @include main(650px);

    div.desc {
        max-width: 650px;
        margin-bottom: 50px;

        h1 {
            @include text($fraunces, $font-size:42px);
        }

        > p {
            margin-top: 25px;
            @include text($inter, $font-size:18px, $line-height:27px);
        }
    }

    div.advanteges {
        @include flex(start, space-between);

        div.content_advanteges {
            max-width: 234.5px;

            h2 {
                @include text($fraunces, $font-size:25px);
                margin: 15px 0;
            }

            p {
                @include text($inter, $font-size:15px, $line-height:24px);
            }
        }
    }
}
</style>