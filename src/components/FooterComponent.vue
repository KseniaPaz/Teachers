<template>
    <div>
        <footer class="footer center">
            <a class="logo" href="index.html">ROBO.SCHOOL <br> <span class="logo__span">© ROBO.SCHOOL</span></a>
            <p class="phone-number">+7 800 000 11 22</p>
        </footer>
    </div>
</template>

<script>
export default {
    name: 'FooterComponent'
}
</script>

<style lang="scss" scoped>
.footer {
    padding-top: 40px;
    padding-bottom: 40px;
    background-color: #141024;
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.logo{
    font-size: 30px;
    font-weight: 700;
    line-height: 48px;
    text-align: left;
    color: #FFFFFF;

    &__span {
        font-family: Jost;
    font-size: 16px;
    font-weight: 400;
    line-height: 25.6px;
    text-align: center;
        color: #FFFFFF;
    }
}

.phone-number {
    font-size: 30px;
    font-weight: 600;
    line-height: 48px;
    text-align: right;
    color: #FFFFFF;
}
</style>