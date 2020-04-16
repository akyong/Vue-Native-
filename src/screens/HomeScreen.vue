<template>
    <view>
        <text class="text-color-primary">{{title}}</text>
<!--        <text>{{aaa}}</text>-->
        <Hello/>
<!--        <button title=" go to screen 1 " :on-press="() =>{ navigate('screen1') }"/>-->
    </view>

</template>


<script>
    import Hello from "@/components/Hello"

    export default {
        components: {
            Hello
        },
        // props: ["aaa","navigate"],
        data() {
            return {
                title: "Home Screen"
            }
        }
    }
</script>


