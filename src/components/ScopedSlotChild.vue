<template>

    <!-- Child Component -->

    <div>
        <slot :user="userDetails">No Data</slot>
    </div>

</template>

<script>

export default {
    name: 'ScopedSlotChild',
    data() {
        return {
            userDetails: {
                name: 'Ayush',
                age: 22,
                edu: 'Bachelors'
            }
        }
    }
}

</script>