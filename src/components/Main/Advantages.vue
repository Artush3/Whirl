<template>
    <section>
        <div class="conteiner_content flex-sb">
            <div class="advantages">
                <img src="..\..\img\Main\Advantages\IMAGE (7).png" alt="advantages1">
                <h2>Fast. Really fast.</h2>
                <p>Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.</p>
            </div>
            <div class="advantages">
                <img src="..\..\img\Main\Advantages\IMAGE (8).png" alt="advantages2">
                <h2>More bang for buck.</h2>
                <p>Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.</p>
            </div>
            <div class="advantages">
                <img src="..\..\img\Main\Advantages\IMAGE (9).png" alt="advantages3">
                <h2>Safe and secure.</h2>
                <p>Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.</p>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: "Advantages"
}
</script>

<style scoped lang="scss">
@use "../../assets/variables.scss" as *;
@use "../../assets/mixins.scss" as *;
section {
    @include main(450px);

    div.advantages {
        padding: 30px;
        min-height: 250px;
        max-width: 355px;

        &:first-of-type {
            background-color: #FAEA73;
        }

        &:nth-child(2) {
            background-color: #CCEFF6;
        }

        &:last-of-type {
            background-color: #F7CEDC;
        }

        h2 {
            margin: 10px 0 15px;
            @include text($fraunces, $font-size:25px, $line-height:31.25px);
        }

        p {
            @include text($inter, $font-size:15px, $line-height:24px);
        }
    }
}
</style>