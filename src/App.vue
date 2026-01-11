<template>
  <div class="taskPlaning">
    <taskPlaning></taskPlaning>
    <mainFuters></mainFuters>
    <caseService></caseService>
  </div>
</template>


<script>
  import taskPlaning from '@/components/taskPlaning.vue';
  import mainFuters from '@/components/mainFuters.vue';
  import caseService from '@/components/caseService.vue';

  export default {
    name: "App",
    components: {
      taskPlaning,
      mainFuters,
      caseService
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
</style>
