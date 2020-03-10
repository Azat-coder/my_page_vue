<template>
  <div class="education"
       v-bind:class="{uppercaseText: isActive=false}">
    <p>С ранних лет я проявлял тягу к естественным наукам, в особенности к биологии. В десятом классе выйграл районно-городскую олимпиаду по биологии, на областной занял шестое место. Ни минуты не раздумывал, на кого пойти учиться.
    Я люблю читать, довольно много уделяю этому времени (профессиональную, художественную и научно-популярную литературу), люблю изучать что-то новое.</p>
    <p>На работе ответственен, стараюсь добиться максимального результата, пунктуален, вежлив.</p>
    <p>С 2018 года я занимаюсь проведением обработок от клещей в весеннее время в качестве подработки. В качестве инструмента для привлечения клиентов создал сайт для своего предприятия. Для этого изучил верстку на уровне достаточном для написания простого одностраничного сайта (HTML, CSS, адаптивную верстку). Сейчас изучаю курсы HTML академии и другие, просто потому, что мне это нравится.</p>
    <p>Люблю заниматься спортом, бегаю по вечерам, занимаюсь на турнике. Люблю футбол. У меня замечательная энтомологическая коллекция.</p>
    <p>Не состою в браке. Детей нет.</p>
    <h2>Образование</h2>
    <ul>
        <education_item
          v-for="education_place of education_places"
          v-bind:key="education_place.id"
          v-bind:education_place="education_place"
         />
    </ul>
  </div>
</template>

<script>
  import education_item from '@/components/education_item'
  

  // data: {
  //   isNav: true,
  //   isActive: true
  // }
  
  

export default {
  name: 'education',
  props: ['education_places'],
  components: {
    education_item
  } 
}



</script>

<style scoped>
 
  ul {
      list-style: none;
      margin: 0;
      padding: 0;
      margin-top: 2em;
  }

  .education {
    margin: 0 auto;
    max-width: 960px;
  }


  .education h2 {
      margin-top: 3em;
      margin-bottom: 2em;
  }
  
  .uppercaseText {
    text-transform: uppercase;
  }

</style>
