<template>

    <!-- Child Element -->
    
    <div style="margin-top: 50px;">

        <!-- Header Part -->
        <slot name="header">No Header Provided</slot>

        <!-- Products Part -->
        <slot name="products">No Product Provided</slot>

        <h1>Lorem, ipsum.</h1>
        <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Incidunt, dolorem?</p>

        <!-- Services Part -->
        <slot name="services">No Service Provided</slot>

        <!-- About Part -->
        <slot name="about">No About Provided</slot>

    </div>
</template>

<script>

export default {
    name: 'NamedSlotChild'
}

</script>