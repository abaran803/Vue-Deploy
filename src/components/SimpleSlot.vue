<template>
    <div>

        <!-- Parent Element -->
        <SimpleSlotChild>

            <!-- Content to be shown in child -->
            <h1>Welcome to Slot Tutorials</h1>
            <p>Here, we'll discuss everything about the slot and their usage</p>
            <hr style="width: 50%;">
            
        </SimpleSlotChild>
    </div>
</template>

<script>
import SimpleSlotChild from './SimpleSlotChild.vue';


export default {
    name: "SimpleSlot",
    components: { SimpleSlotChild }
}

</script>