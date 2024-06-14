<template>
    <div>
        <section class="price center" id="section_price">
        <h2 class="price__heading">Выберите нужный пакет</h2>
        <div class="price__box">
            <div class="price__item">
                <h3 class="price__item_title">– PRO –</h3>
                <p class="price__item_sum">20.000 ₽</p>
                <p class="price__item_text">УМК по робототетхнике и программированию</p>
                <a href="#section_subscribe" class="price__item_button">Оставить заявку</a>
            </div>

            <div class="price__item">
                <h3 class="price__item_title">– ROBO –</h3>
                <p class="price__item_sum">15.000 ₽</p>
                <p class="price__item_text">УМК по робототетхнике </p>
                <a href="#section_subscribe" class="price__item_button">Оставить заявку</a>
            </div>

            <div class="price__item">
                <h3 class="price__item_title">– PROG –</h3>
                <p class="price__item_sum">10.000 ₽</p>
                <p class="price__item_text">УМК по программированию</p>
                <a href="#section_subscribe" class="price__item_button">Оставить заявку</a>
            </div>
        </div>
    </section>
    </div>
</template>

<script>
export default {
    name: 'PriceComponent'
}
</script>

<style lang="scss" scoped>
.price {
    padding-top: 120px;
    padding-bottom: 120px;
    padding-left: 180px;
    display: flex;
    flex-direction: column;
    gap: 60px;

    &__heading {
        font-size: 50px;
        font-weight: 600;
        line-height: 80px;
        text-align: left;
        color: #141024;
    }

    &__box {
        display: grid;
        grid-template-columns: repeat(3, 360px);
        gap: 40px;
    }

    &__item {
        padding-top: 40px;
        padding-bottom: 40px;
        border: 1px solid #14102433;
        border-radius: 16px;
        display: flex;
        flex-direction: column;
        align-items: center;

        &_title {
            font-size: 30px;
            font-weight: 600;
            line-height: 48px;
            text-align: center;
            color: #141024;
            margin-bottom: 68px;
        }

        &_sum {
            font-size: 50px;
            font-weight: 600;
            line-height: 80px;
            text-align: center;
            color: #141024;
            margin-bottom: 25px;
        }

        &_text {
            width: 250px;
            height: 60px;
            font-weight: 400;
            line-height: 28.8px;
            text-align: center;
            color: #141024;
            margin-bottom: 61px;
        }

        &_button {
            display: flex;
            justify-content: center;
            align-items: center;
            width: 280px;
            height: 79px;
            border:none;
            border-radius: 5px;
            background-color: #D52027;
            font-size: 18px;
            font-weight: 400;
            line-height: 28.8px;
            color: #FFFFFF;
        }
    }
}

.price__item:hover {
    background-color: #141024;
}

.price__item:hover .price__item_title{
    color: #FFFFFF;
}

.price__item:hover .price__item_text{
    color: #FFFFFF;
}

.price__item:hover .price__item_sum{
    color: #FFFFFF;
}
</style>