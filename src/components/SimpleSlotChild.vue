<template>

    <!-- Child Element -->
    <div>

        <!-- The wrapped content will show here -->
        <slot></slot>

        <div style="color: green;">
            The above part is the content wrapped b/w the child element of its parent.
        </div>
    </div>
</template>

<script>

export default {
    name: 'SimpleSlotChild'
}

</script>