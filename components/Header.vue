<template>
    <nb-container>
        <nb-header :style="styles.header_background">
            <nb-left>
                <nb-button transparent>

                    <nb-text :style="styles.header_background">Back</nb-text>
                </nb-button>
            </nb-left>
            <nb-body>
                <nb-title :style="{color: '#FA0'}">Header</nb-title>
            </nb-body>
            <nb-right>
                <nb-button transparent>
                    <nb-text :style="styles.header_background" >Cancel</nb-text>
                </nb-button>
            </nb-right>
        </nb-header>
    </nb-container>
</template>

<script>
    import sadis_styles from "../assets/js/sadis_styles.js";

    export default {
        computed:{
            styles: function(){
                return sadis_styles;
            }
        }
    }
</script>