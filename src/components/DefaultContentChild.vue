<template>

    <!-- Child Element -->
    <div>

        <!-- The wrapped content will show here -->
        <slot>
            <div style="color: red; margin-top: 20px">
                This red text will load only when there is no content wrapped
            </div>
        </slot>

    </div>
</template>

<script>

export default {
    name: 'DefaultContentChild'
}

</script>