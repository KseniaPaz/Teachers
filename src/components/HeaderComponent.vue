<template>
    <div>
        <header class="header center">
            <div class="header__head">
                <a class="logo" href="index.html">ROBO.SCHOOL</a>
                <nav class="menu">
                    <a href="#section_info" class="menu__link">О школе</a>
                    <a href="#section_teachers" class="menu__link">Тренеры</a>
                    <a href="#section_price" class="menu__link">Стоимость</a>
                </nav>
                <p class="phone-number">+7 800 000 11 22</p>
            </div>
            <div class="top">
                <div class="top__left">
                    <h1 class="top__left__title">ROBO SCHOOL</h1>
                    <p class="top__left__text">Курсы повышения квалификации по робототехнике для педагогов начальной школы
                    </p>
                    <a href="#section_subscribe" class="top__left__button">Записаться на курс</a>
                </div>
                <div class="top__right"><img class="top__img" src="../assets/img/Top-image.png" alt="top__img"></div>
            </div>
        </header>
    </div>
</template>

<script>
export default {
    name: 'HeaderComponent',
}
</script>

<style lang="scss" scoped>

.header {
    background-color: #141024;

    &__head {
        display: flex;
        justify-content: space-between;
        align-items: center;
        padding-top: 30px;
    }
}

.logo{
    font-size: 30px;
    font-weight: 700;
    line-height: 48px;
    text-align: left;
    color: #FFFFFF;
}

.menu {
    width: 342px;
    display: flex;
    gap: 40px;
    &__link {
        font-size: 20px;
        font-weight: 400;
        line-height: 32px;
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

.top {
    margin-top: 84px;
    display: flex;
    justify-content: center;

    &__left {
        padding-top: 174px;
        padding-left: 120px;
        width: 516px;
        display: flex;
        flex-direction: column;
        gap: 50px;
        &__title {
            width: 516px;
            font-size: 70px;
            font-weight: 600;
            line-height: 112px;
            text-align: left;
            color: #FFFFFF;
        }
        &__text {
            font-size: 20px;
            font-weight: 400;
            line-height: 32px;
            text-align: left;
            color: #FFFFFF;
        }
        &__button {
            display: flex;
            align-items: center;
            justify-content: center;
            width: 260px;
            height: 79px;
            border-radius: 5px;
            background: #D52027;
            border: none;
            font-size: 18px;
            font-weight: 400;
            line-height: 18px;
            color: #FFFFFF;
        }
        &__button:hover {
            background: #b11318;
        }
    }

    &__right {
        max-width: 783px;
        max-height: 918px;
    }
    &__img{
        max-width: 783px;
        max-height: 918px;
    }
}
</style>