<template>
    <view>
        <text class="text-color-primary">{{title}}</text>
        <!--        <button title=" go to Home Screen " :on-press="() =>{ navigate('homeScreen') }"/>-->
    </view>

</template>

<style>
    .container {
        background-color: white;
        align-items: center;
        justify-content: center;
        flex: 1;
    }
    .text-color-primary {
        color: blue;
    }
</style>

<script>

    export default {
        data() {
            return {
                title: "Screen 2"
            }
        }
    }
</script>


