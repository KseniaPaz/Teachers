<template>
    <div class="popup_wrapper">
        <div class="v-popup" center>
            <div class="v-popup__header">
                <span>
                    <i 
                        class="material-icons"
                        @click="closePopup"
                    >
                        close
                    </i>
                </span>
            </div>
            <div class="v-popup__content">
                <slot></slot>
            </div>
        </div>
        
    </div>
</template>

<script>
export default {
    name: 'TePopUp',
    props: {},
    data() {
        return {
            
        }
    },
    methods: {
        closePopup() {
            this.$emit('closePopup')
        }
    }
}
</script>

<style lang="scss" scoped>
.popup_wrapper {
    display: flex;
    justify-content: center;
    align-items: center;
    position: absolute;
    right: 0;
    left: 0;
    top: 0;
    bottom: 0;
}

.v-popup {
    overflow-y: scroll;
    position: fixed;
    top: 30px;
    border-radius: 12px;
    background: #fff;
    box-shadow: 0 0 17px 0 #e7e7e7;
    width: 940px;
    height: 512px; 
    padding: 16px;
    z-index: 10;
    &__header {
        display: flex;
        justify-content: flex-end;
    }
    &__content {
        display: flex;
        flex-direction: column;
    }
}
    
</style>