<template>
    <section>
        <div class="conteiner_content flex-sb">
            <img src="C:\Users\user\Desktop\Whirl\whirl\src\img\Main\Set\IMAGE (13).png" alt="фото">
            <div class="desc">
                <h1>Set, forget, and then<br> track.</h1>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit,<br> sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</p>
                <div class="advantages">
                    <img src="C:\Users\user\Desktop\Whirl\whirl\src\img\Main\Set\Vector.png" alt="advantages">
                    <p>Understand your options</p>
                </div>
                <div class="advantages">
                    <img src="C:\Users\user\Desktop\Whirl\whirl\src\img\Main\Set\Vector.png" alt="advantages">
                    <p>No lock-ins</p>
                </div>
                <div class="advantages">
                    <img src="C:\Users\user\Desktop\Whirl\whirl\src\img\Main\Set\Vector.png" alt="advantages">
                    <p>You own the shares</p>
                </div>
                <button><a href="#">Book a demo</a></button>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: "Set"
}
</script>

<style scoped lang="scss">
@use "../../assets/mixins.scss" as *;
@use "../../assets/variables.scss" as *;
section {
    @include main(550px, #0070A0);

    div.desc {
        max-width: 501px;

        h1 {
            @include text($fraunces, $font-size:42px, $line-height:50.4px, $color:#FFFFFF);
        }

        > p {
            margin: 10px 0 20px;
            @include text($inter, $font-size:18px, $line-height:27px, $color:#FFFFFF);
        }

        div.advantages {
            @include flex(center);
            margin-bottom: 10px;

            p {
                margin-left: 10px;
                @include text($inter, $line-height:21.6px, $color:#FFFFFF);
            }
        }

        button {
            @include button-a(43px, 176px, #0070A0, #FFFFFF);
        }
    }
}
</style>