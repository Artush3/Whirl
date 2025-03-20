<template>
    <section>
        <div class="conteiner_content">
            <h1>We will take care of everything,<br> <span>so you can get back to relaxing.</span></h1>
            <div class="desc">
                <img src="C:\Users\user\Desktop\Whirl\whirl\src\img\Main\Care\Frame.png" alt="вкладки">
                <img src="C:\Users\user\Desktop\Whirl\whirl\src\img\Main\Care\IMAGE (10).png" alt="картина">
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: "Care"
}
</script>

<style scoped lang="scss">
@use "../../assets/mixins.scss" as *;
@use "../../assets/variables.scss" as *;
section {
    @include main(800px);
    
    h1 {
        @include text($fraunces, $font-size:42px, $line-height:50.4px);

        span {
            @include text($fraunces, $font-size:39px, $line-height:50.4px);
        }
    }

    div.desc {
        @include flex(center, space-between);
    }
}
</style>