<template>
  <div class="taskPlaning">
    <taskPlaning></taskPlaning>
    <mainFuters></mainFuters>
    <caseService></caseService>
  </div>
  <div class="cards-list">
    <cardsList 
    v-for="value in cards"
    :index="value.index"
    :title="value.title"
    :text="value.text"
    :key="value.cards">
    </cardsList>
  </div>
  <div class="whereUses">
    <h2>Где можно использовать</h2>
    <whereUse 
    v-for="value in whereUses"
    :title_use="value.title_use"
    :text_use="value.text_use"
    :buttons_use="value.buttons_use"
    :key="value.whereUses">
    </whereUse>
  </div>
</template>


<script>
  import taskPlaning from '@/components/taskPlaning.vue';
  import mainFuters from '@/components/mainFuters.vue';
  import caseService from '@/components/caseService.vue';
  import cardsList from '@/components/cardsList.vue';
  import whereUse from '@/components/whereUse.vue';



  export default {
    name: "App",
    components: {
      taskPlaning,
      mainFuters,
      caseService,
      cardsList,
      whereUse
    },
    data () {
      return {
        cards: [
          {
            index: '1',
            title: 'Добавьте задачи',
            text: 'Запишите всё, что нужно сделать.'
          },
          {
            index: '2',
            title: 'Назначьте приоритет',
            text: 'Отметьте важные и срочные дела.',
          },
          {
            index: '3',
            title: 'Выполняйте',
            text: 'Закрывайте задачи без хаоса.',
          }
        ],
        whereUses: [
          {
            title_use: 'Учёба',
            text_use: 'Помогает не пропускать дедлайны.',
            buttons_use: [
              'Домашка', 
              'Экзамены', 
              'Проекты', 
              'Конспекты', 
              'Курсы'
            ]
          },
          {
            title_use: 'Личные дела',
            text_use: 'Упрощает бытовые и повседневные задачи.',
            buttons_use: [
              'Покупки', 
              'Уборка', 
              'Финансы', 
              'Финансы', 
              'Планы'
            ]
          }
        ]
      }
    }
  }
</script>


<style>
  @import url('https://fonts.googleapis.com/css2?family=Source+Code+Pro:ital,wght@0,200..900;1,200..900&display=swap');

  * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: "SourceCodePro", monospace;
      font-optical-sizing: auto;
      font-style: normal;
  }
  body {
    background-color: #F5F5F5;
  }
  .taskPlaning {
    display: flex;
    flex-direction: row;
  }
  .cards-list {
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
    justify-content: flex-start;
  }
</style>
