<template>
    <view>
        <text class="text-color-primary">{{message}}</text>
        <button :title="btnMessage" :on-press="handlerClick"/>
        <text>{{clickcount}}</text>
        <text>{{clickMutasi}}</text>
    </view>
</template>

<script>
    export default {
        data(){
            return {
                message: "Welcome to my application baby",
                btnMessage: "Tekan Aku",
                clickcount: 0
            }
        },
        methods:{
            handlerClick() {
                this.clickcount+=1;
            }
        },
        computed:{
            clickMutasi(){
                if(this.clickcount < 5){
                    return "Tekan lagi, batas adalah 4";
                }
                else{
                    return "mantap betul lah pokoknya!!"
                }
            }
        }
    }
</script>

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