<template>
    <section>
        <div class="conteiner">
            <h1>Trusted by 50,000+ companies</h1>
            <div class="companies">
                <img src="C:\Users\user\Desktop\Whirl\whirl\src\img\Main\Companies\IMAGE (3).png" alt="companies1">
                <img src="C:\Users\user\Desktop\Whirl\whirl\src\img\Main\Companies\IMAGE (4).png" alt="companies2">
                <img src="C:\Users\user\Desktop\Whirl\whirl\src\img\Main\Companies\IMAGE (5).png" alt="companies3">
                <img src="C:\Users\user\Desktop\Whirl\whirl\src\img\Main\Companies\IMAGE (6).png" alt="companies4">
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: "Companies"
}
</script>

<style scoped lang="scss">
@use "../../assets/variables.scss" as *;
@use "../../assets/mixins.scss" as *;
section {
    @include main(180px);
    text-align: center;

    h1 {
        @include text($inter, $font-size:24px, $line-height:37.5px);
        margin-bottom: 15px;
    }

    div.companies {
        width: 700px;
        @include flex(center, space-between);
    }
}
</style>