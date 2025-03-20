<template>
    <section>
        <div class="conteiner_content">
            <h1>What's Whirl all about?</h1>
            <div class="about">
                <div class="about_content">
                    <h2>All on one place.</h2>
                    <p>Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.</p>
                </div>
                <div class="about_content">
                    <img src="C:\Users\user\Desktop\Whirl\whirl\src\img\Main\Whats\IMAGE (11).png" alt="about1">
                    <h2>Get daily alerts.</h2>
                    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore.</p>
                </div>
                <div class="about_content">
                    <img src="C:\Users\user\Desktop\Whirl\whirl\src\img\Main\Whats\IMAGE (12).png" alt="about2">
                    <h2>Safe and secure.</h2>
                    <p>Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.</p>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: "Whats"
}
</script>

<style scoped lang="scss">
@use "../../assets/mixins.scss" as *;
@use "../../assets/variables.scss" as *;
section {
    @include main(450px);

    div.conteiner_content {
        @include flex(start, space-between);

        h1 {
            @include text($fraunces, $font-size:42px, $line-height:50.4px);
            width: 300px;
        }

        div.about {
            width: 732px;
            @include flex(end, space-between);

            div.about_content {
                max-width: 223px;

                h2 {
                    margin: 10px 0;
                    @include text($fraunces, $font-size:25px, $line-height:31.25px);
                }

                p {
                    @include text($inter, $font-size:15px, $line-height:24px);
                }
            }
        }
    }
}
</style>