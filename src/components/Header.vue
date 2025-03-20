<template>
    <header>
        <div class="conteiner_content flex-sb">
            <div class="way_content">
                <img src="C:\Users\user\Desktop\Whirl\whirl\src\img\Header\IMAGE.png" alt="logo">
                <nav class="nav_content">
                    <a href="#">Features</a>
                    <a href="#">Pricing</a>
                    <a href="#">Integrations</a>
                    <a href="#">Learn</a>
                </nav>
            </div>
            <div class="user_content">
                <a href="#">Sign in</a>
                <button><a href="#">Book a demo</a></button>
            </div>
        </div>
    </header>
</template>

<script>
export default {
    name: "Header"
}
</script>

<style scoped lang="scss">
@use "../assets/mixins.scss" as *;
@use "../assets/variables.scss" as *;
header {
    @include main(75px);

    div.way_content {
        @include flex(center);

        nav.nav_content {
            margin-left: 30px;
            a {
                &:not(:first-of-type) {
                    margin-left: 25px;
                }

                @include text($inter, $font-size:15px, $line-height:24px, $color:#33383F);
            }
        }
    }

    div.user_content {
        > a {
            @include text($inter, $font-size:15px, $line-height:24px, $color:#0070A0);
        }

        button {
            margin-left: 30px;
            @include button-a(36px, 139px, #0070A0, #FFFFFF, 15px);
        }
    }
}
</style>