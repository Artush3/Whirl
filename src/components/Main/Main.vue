<template>
    <main>
        <Automation></Automation>
        <Compamies></Compamies>
        <Advantages></Advantages>
        <Care></Care>
        <Whats></Whats>
        <Set></Set>
        <Automated></Automated>
        <Blog></Blog>
        <Start></Start>
    </main>
</template>

<script>
import Automation from './Automation.vue';
import Compamies from './Compamies.vue';
import Advantages from './Advantages.vue';
import Care from './Care.vue';
import Whats from './Whats.vue';
import Set from './Set.vue';
import Automated from './Automated.vue';
import Blog from './Blog.vue';
import Start from './Start.vue';
export default {
    name: "Main",
    components: { Automation, Compamies, Advantages, Care, Whats, Set, Automated, Blog, Start }
}
</script>