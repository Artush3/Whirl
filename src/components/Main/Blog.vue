<template>
    <section>
        <div class="conteiner_content">
            <div class="nav">
                <h1>Get smarter, with our blog.</h1>
                <a href="#">See All Posts</a>
            </div>
            <div class="blog">
                <div class="blog_content">
                    <img src="C:\Users\user\Desktop\Whirl\whirl\src\img\Main\Blog\IMAGE (15).png" alt="фото">
                    <div class="desc_content">
                        <p>Improvements</p>
                        <h2>Automating Daily Tasks from Your Phone</h2>
                        <p>Dicta nihil ratione corrupti. Aut dolorem dolores omnis laboriosam ratione sequi. Provident ad sed velit. Est ea ab.</p>
                        <p>April 24, 2022</p>
                    </div>
                </div>
                <div class="blog_content">
                    <img src="C:\Users\user\Desktop\Whirl\whirl\src\img\Main\Blog\IMAGE (16).png" alt="фото">
                    <div class="desc_content">
                        <p>Tips & Tricks</p>
                        <h2>Can You Automate Group Learning?</h2>
                        <p>Dicta nihil ratione corrupti. Aut dolorem dolores omnis laboriosam ratione sequi. Provident ad sed velit. Est ea ab.</p>
                        <p>April 24, 2022</p>
                    </div>
                </div>
                <div class="blog_content">
                    <img src="C:\Users\user\Desktop\Whirl\whirl\src\img\Main\Blog\IMAGE (17).png" alt="фото">
                    <div class="desc_content">
                        <p>News</p>
                        <h2>Our $3,000,000 B Round Investors</h2>
                        <p>Eos ipsum et est quis neque cum. Quis autem est eligendi amet animi eaque. Itaque minus illo delectus vel vitae dolores minus.</p>
                        <p>April 24, 2022</p>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: "Blog"
}
</script>

<style scoped lang="scss">
@use "../../assets/mixins.scss" as *;
@use "../../assets/variables.scss" as *;
section {
    @include main(750px);

    div.nav {
        margin-bottom: 50px;
        @include flex(center, space-between);

        h1 {
            @include text($fraunces, $font-size:42px);
        }

        a {
            @include text($inter, $font-size:17px, $color:#0070A0);
        }
    }

    div.blog {
        @include flex(center, space-between);

        div.blog_content {
            max-width: 355px;

            div.desc_content {
                padding: 25px;

                p {
                    &:first-of-type {
                        margin-bottom: 10px;
                        width: max-content;
                        background-color: #E6F7FF;
                        padding: 5px 15px;
                        @include text($inter, $font-size:12px, $color:#2C90C9);
                    }

                    &:not(:first-of-type):not(:last-of-type) {
                        margin: 20px 0;
                        @include text($inter, $font-size:14px, $line-height:19.6px);
                    }

                    &:last-of-type {
                        @include text($inter, $font-size:12px);
                    }
                }

                h2 {
                    @include text($fraunces, $font-size:25px, $line-height:31.25px);
                }
            }
        }
    }
}
</style>