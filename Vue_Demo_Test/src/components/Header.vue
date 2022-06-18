<script>
import { ref } from "vue";
export default {
    // setup() {
    //     const isVisible = ref(false);
    //     function toggle() {
    //         this.isVisible = !this.isVisible;
    //         console.log(this.isVisible)
    //     }
    //     return {
    //         toggle,
    //         isVisible,
    //     };
    // },
    // ------------------------------------------------------------
    setup() {
        function toggle() {
            const modal = document.querySelector(".modal");
            if(modal.style.display == "none"){
                modal.style.display = "block"
            } else{
                modal.style.display = "none"
            }
            console.log(modal);
        }
        return {
            toggle,
        };
    },
};
</script>

<template>
    <!-- <div class="test">
        <div class="container">
            <button id="modal-button" v-on:click="toggle">Click me</button>
        </div>
        <div class="modal" v-if="isVisible"></div>
    </div> -->
    <!-- ----------------------------------------------------------------- -->
    <div class="test">
        <div class="container">
            <button id="modal-button" v-on:click="toggle">Click me</button>
        </div>
        <div class="modal"></div>
    </div>
</template>

<style>
.test {
    height: 100vh;
    width: 100vw;
}

.container {
    background-color: gray;
    width: 80%;
    height: 80%;
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
}

.modal {
    position: fixed;
    height: 20%;
    width: 20%;
    background-color: red;
}
</style>
