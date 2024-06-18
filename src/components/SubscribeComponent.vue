<template>
    <div>
        <section class="subscribe center" id="section_subscribe">
        <img class="subscribe__mask" src="../assets/img/Mask Group.png" alt="Mask">
        <div class="subscribe__box">
            <h2 class="subscribe__box_heading">Запишитесь на курс со скидкой 10%</h2>
            <p class="subscribe__box_text">Акция действительна до 10 марта 2022 года</p>
        </div>
        <form class="forma" action="#" method="post">
            <input class="forma__input" type="text" required placeholder="Имя">
            <input class="forma__input" type="tel" required placeholder="Телефон">
            <input class="forma__input" type="email" required placeholder="E-mail">
            <button class="forma__button" type="submit">Оформить заявку</button>
        </form>
    </section>
    </div>
</template>

<script>
export default {
    name: 'SubscribeComponent'
}
</script>

<style lang="scss" scoped>
.subscribe {
    position: relative;
    padding-top: 87px;
    padding-bottom: 100px;
    display: flex;
    justify-content: center;
    gap: 144px;
    background-color: #D52027;
    &__box {
        padding-top: 19px;
        display: flex;
        flex-direction: column;
        gap: 20px;
        &_heading {
            width: 400px;
            font-size: 36px;
            font-weight: 600;
            line-height: 46.8px;
            text-align: left;
            color: #FFFFFF;
        }
        &_text {
            font-size: 20px;
            font-weight: 400;
            line-height: 26px;
            text-align: left;
            color: #FFFFFF;
        }
    }
    &__mask {
        position: absolute;
        top: 11px;
        left: 1px;
    }
  }
.forma {
    display: flex;
    flex-direction: column;
    gap: 10px;
    z-index: 10;
    &__input{
        padding-left: 20px;
        width: 480px;
        height: 64px;
        border: none;
        border-radius: 5px;
        font-size: 18px;
        font-weight: 400;
        line-height: 26.01px;
        text-align: left;
        color: #282944B2;
    }
    &__button {
        width: 500px;
        height: 64px;
        border: none;
        border-radius: 5px;
        background-color: #141024;
        font-size: 18px;
        font-weight: 400;
        line-height: 26.01px;
        text-align: center;
        color: #FFFFFF;
    }
}
</style>