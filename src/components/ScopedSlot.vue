<template>

    <div>

    <!-- Parent Component -->
    
    <ScopedSlotChild v-slot="slotProps">
        <div style="margin-top: 30px;">
            {{ slotProps.user.name }} |
            {{ slotProps.user.age }} |
            {{ slotProps.user.edu }}
        </div>
    </ScopedSlotChild>

    </div>

</template>

<script>
import ScopedSlotChild from './ScopedSlotChild.vue';


export default {
    name: "ScopedSlot",
    components: { ScopedSlotChild }
}

</script>