<template>
    <div>

        <!-- Parent Element -->

        <NamedSlotChild>

            <!-- Header Part -->
            <template v-slot:header>
                <ul type="none">
                    <li>Home</li>
                    <li>Produts</li>
                    <li>Services</li>
                    <li>About Us</li>
                </ul>
            </template>

            
            <!-- About -->
            <template v-slot:about>
                <h1><u>About Us</u></h1>
                <p style="width: 60%; margin: auto;">
                    Lorem ipsum dolor sit amet consectetur adipisicing elit. Accusantium debitis sint inventore quasi dolore omnis nobis illo sed commodi deserunt, vitae perferendis    reiciendis tempore dolorem reprehenderit alias distinctio suscipit praesentium?
                </p>
            </template>

            <!-- Services -->
            <template #services>
                <h1><u>Services</u></h1>
                <div class="items">
                    <div class="item">
                        <div v-for="e in images" :key="e" :style="`background: url(${e}) center center/cover; width: 200px; height: 200px; border: 1px solid black;`"></div>
                    </div>
                </div>
            </template>

            <!-- Products -->
            <template #products>
                <h1><u>Products</u></h1>
                <div class="items">
                    <div class="item">
                        <div v-for="e in imagesB" :key="e" :style="`background: url(${e}) center center/cover; width: 200px; height: 200px; border: 1px solid black;`"></div>
                    </div>
                </div>
            </template>

        </NamedSlotChild>

    </div>
</template>

<script>
import NamedSlotChild from './NamedSlotChild.vue';
import image1 from '../assets/services/image1.jpg';
import image2 from '../assets/services/image3.jpg';
import image3 from '../assets/services/image2.jpg';
import image4 from '../assets/products/image1.jpg';
import image5 from '../assets/products/image3.jpg';
import image6 from '../assets/products/image2.jpg';

export default {
    name: "NamedSlot",
    components: { 
        NamedSlotChild,
    },
    data() {
        return {
            images: [image1, image2, image3],
            imagesB: [image4, image5, image6]
        }
    }
}

</script>

<style scoped>

ul {
    display: flex;
    padding: 10px;
    margin: 0;
    color: rgb(164, 107, 0);
    border-bottom: 1px solid orange;
    position: fixed;
    width: 100%;
    top: 0;
    background-color: rgb(255, 249, 238);
}

li {
    margin-left: 25px;
    font-weight: 600;
    font-size: 20px;
    cursor: pointer;
    padding: 4px 6px;
    border-radius: 5px;
}

li:hover {
    background-color: orange;
    color: white;
}

.item {
    display: flex;
    gap: 20px;
    justify-content: center;
}

.items {
    margin-bottom: 50px;
}

</style>