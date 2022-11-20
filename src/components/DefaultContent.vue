<template>
    <div>

        <!-- Parent Element -->

        <!-- Default/Fallback content -->
        <DefaultContentChild />

    </div>
</template>

<script>
import DefaultContentChild from './DefaultContentChild.vue';


export default {
    name: "DefaultContent",
    components: { DefaultContentChild }
}

</script>