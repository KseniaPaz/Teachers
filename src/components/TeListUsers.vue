<template>
    <div>
        <section class="teachers center" id='section_teachers'>
            <h3 class="teachers__heading">Профессиональные тренеры</h3>

            <TeCarousel
            :carousel_data="listUsers"
            />
        </section>
        

    </div>
</template>

<script>
import TeCarousel from './TeCarousel.vue'


export default {
    name: 'TeListUsers',
    components: {TeCarousel},

    data() {
            return {
                listUsers: [
                    {
                        id: 1,
                        image: 'photo1.jpg',
                        name: 'Ирина Лайм',
                        prof: 'преподаватель по робототехнике',
                        educationDate: 'Сентябрь 1995 — Июнь 2000',
                        educationPlace: 'Санкт-Петербургский политехнический университет Петра Великого',
                        faculty: 'Факультет: Компьютерных наук и технологий',
                        speciality: 'Специальность: Математика и компьютерные науки',
                        formOfEducstion: 'Форма обучения: Очная'               
                    },

                    {
                        id: 2,
                        image: 'photo2.jpg',
                        name: 'Марина Орлова',
                        prof: 'преподаватель по робототехнике',
                        educationDate: 'Сентябрь 1995 — Июнь 2000',
                        educationPlace: 'Санкт-Петербургский политехнический университет Петра Великого',
                        faculty: 'Факультет: Компьютерных наук и технологий',
                        speciality: 'Специальность: Математика и компьютерные науки',
                        formOfEducstion: 'Форма обучения: Очная'
                    },

                    {
                        id: 3,
                        image: 'photo3.jpg',
                        name: 'Максим Петров',
                        prof: 'преподаватель по программированию',
                        educationDate: 'Сентябрь 1995 — Июнь 2000',
                        educationPlace: 'Санкт-Петербургский политехнический университет Петра Великого',
                        faculty: 'Факультет: Компьютерных наук и технологий',
                        speciality: 'Специальность: Математика и компьютерные науки',
                        formOfEducstion: 'Форма обучения: Очная'
                    },

                    {
                        id: 4,
                        image: 'photo4.jpg',
                        name: 'Константин Назаров',
                        prof: 'преподаватель по робототехнике',
                        educationDate: 'Сентябрь 1995 — Июнь 2000',
                        educationPlace: 'Санкт-Петербургский политехнический университет Петра Великого',
                        faculty: 'Факультет: Компьютерных наук и технологий',
                        speciality: 'Специальность: Математика и компьютерные науки',
                        formOfEducstion: 'Форма обучения: Очная'
                    },

                    {
                        id: 5,
                        image: 'photo5.jpg',
                        name: 'Лиза Весенняя',
                        prof: 'преподаватель по программированию',
                        educationDate: 'Сентябрь 1995 — Июнь 2000',
                        educationPlace: 'Санкт-Петербургский политехнический университет Петра Великого',
                        faculty: 'Факультет: Компьютерных наук и технологий',
                        speciality: 'Специальность: Математика и компьютерные науки',
                        formOfEducstion: 'Форма обучения: Очная'
                    },
                ]
            }
    },

    

    methods: {
        showTUserIdInConsole(data) {
            console.log(data);
        }
    },
    }
</script>

<style lang="scss" scoped>

.teachers {
    padding-top: 16px;
    padding-bottom: 16px;
    padding-left: 180px;

    &__box {
        padding-top: 60px;
        display: grid;
        grid-template-columns: repeat(6, 360px);
        gap: 40px;
    }

    &__item {
      display: flex;
      flex-direction: column;
      gap: 20px;
    }

    &__name {
      font-size: 24px;
      font-weight: 600;
      line-height: 38.4px;
      text-align: left;
      color: #141024;
    }

    &__prof {
      font-size: 18px;
      font-weight: 400;
      line-height: 28.8px;
      text-align: left;
      color: #141024B2;
    }

    &__next {
      font-size: 18px;
      font-weight: 400;
      line-height: 28.8px;
      text-align: left;
      color: #D52027;
    }
  }

   .button__box {
    display: flex;
    margin-top: 60px;
    gap: 10px;
    justify-content: flex-end;
  } 

  .teachers__heading {
    margin-bottom: 16px;
    font-size: 50px;
    font-weight: 600;
    line-height: 80px;
    text-align: left;
    color: #141024;
  }

</style>