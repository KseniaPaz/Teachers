<template>
    <div>
        <section class="info center" id="section_info">
            <div class="info__about">
                <p class="info__about__text"><span class="info__about__text_span">Robo School</span> – учреждение для
                    формирования кадрового педагогического резерва в сфере робототехникии программирования</p>
                <div class="info__about__box">
                    <div class="info__about__numbers">
                        <p class="info__about__numbers_num">10</p>
                        <p class="info__about__numbers_text">УМК по различным направлениям по робототехнике</p>
                    </div>
                    <div class="info__about__numbers">
                        <p class="info__about__numbers_num">20</p>
                        <p class="info__about__numbers_text">Школ, в которых запущена робототехника</p>
                    </div>
                    <div class="info__about__numbers">
                        <p class="info__about__numbers_num">100</p>
                        <p class="info__about__numbers_text">Педагогов прошедших курсы повышения квалификации</p>
                    </div>
                    <div class="info__about__numbers">
                        <p class="info__about__numbers_num">10 000</p>
                        <p class="info__about__numbers_text">Обученных детей на базе собственных центров</p>
                    </div>
    
                </div>
            </div>
    
            <div class="info__after">
                <p class="info__after__text">Что вы получите после курса</p>
                <div class="info__after__box">
                    <img class="info__icon" src="../assets/img/i.svg" alt="i">
                    <div class="info__hint">
                        <p class="info__hint_text">При наличии свободных мест</p>
                    </div>
                    <div class="info__after__items">
                        <h3 class="info__after__items_title">Удостоверение</h3>
                        <p class="info__after__items_text">Дающее право преподавать робототехнику для детей 6-12 лет в
                            образовательных учреждениях</p>
                    </div>
                    <div class="info__after__items">
                        <h3 class="info__after__items_title">Знания</h3>
                        <p class="info__after__items_text">По основам разработки учебно-методических комплексов
                            по робототехнике и программированию</p>
                    </div>
                    <div class="info__after__items">
                        <h3 class="info__after__items_title">Практику</h3>
                        <p class="info__after__items_text">Возможность пройти практику по преподаванию робототехники на базе
                            R:ED LAB (в оффлайн или онлайн формате)</p>
                    </div>
                </div>
            </div>
        </section>
    </div>
</template>

<script>
export default {
    name: 'InfoComponent'
}
</script>

<style lang="scss" scoped>
    .info {
        padding-top: 120px;
        display: flex;
        flex-direction: column;

        &__about {
        padding-left: 180px;
        margin-bottom: 120px;
        min-width: 1046px;
        display: flex;
        flex-direction: column;
        gap: 60px;

        &__text {
            width: 891px;
            font-size: 30px;
            font-weight: 400;
            line-height: 48px;
            text-align: left;
            color: #141024;

            &_span {
            font-weight: 600;
            }
        }

        &__box {
            display: flex;
            gap: 40px;
        }

        &__numbers {
            max-width: 236px;
            display: flex;
            flex-direction: column;
            gap: 20px;

            &_num {
            font-size: 70px;
            font-weight: 600;
            line-height: 112px;
            text-align: left;
            color: #D52027;
            }

            &_text {
            font-size: 18px;
            font-weight: 400;
            line-height: 28.8px;
            text-align: left;
            color: #141024B2;
            }
        }

        }

    }

    .info__after {
        position: relative;
        padding-top: 100px;
        padding-bottom: 100px;
        padding-left: 180px;
        width: 1046px;
        display: flex;
        flex-direction: column;
        gap: 60px;
        
        &__text {
        font-size: 50px;
        font-weight: 600;
        line-height: 80px;
        text-align: left;
        color: #141024;
        }

        &__box {
        display: flex;
        gap: 40px;
        }

        &__items {
        max-width: 360px;
        display: flex;
        flex-direction: column;
        gap: 20px;

        &_title {
            font-size: 24px;
            font-weight: 600;
            line-height: 38.4px;
            text-align: left;
            color: #141024;
        }

        &_text {
            font-size: 18px;
            font-weight: 400;
            line-height: 28.8px;
            text-align: left;
            color: #141024;
        }

        }

    }

    .info__icon {
    position: absolute;
    right: 220px;
    }

    .info__hint {
    opacity: 0;
    display: flex;
    align-items: center;
    justify-content: center;
    width: 251px;
    height: 56px;
    border-radius: 5px;
    box-shadow: 0px 2px 8px 0px #1410241A;
    position: absolute;
    right: 10px;
    top: 170px;

    &_text {
        font-size: 16px;
        font-weight: 400;
        line-height: 16px;
        text-align: center;
        color:#141024;
    }
    }

    .info__icon:hover ~.info__hint {
    opacity: 1;
    }

</style>