<template>
  <div class="work" 
  v-bind:class="{darkTheme: isDark}"
  @colorChanged="darkTheme = true"
  >
    <div class="container">
    <h1>Опыт работы</h1>
				<table>
          <tr>
            <td>Февраль 2018 — настоящее время</td>
            <td>ЧОБУ "Красноармейское лесничество", Челябинск<br>
            <b>инженер по лесовосстановлению</b><br>
              <ul>
                <li>организация и координация комплекса работ по лесовосстановлению</li>
                <li>организация и координация работы лесного питомника ЧОБУ "Красноармейское лесничество"</li>
                <li>сдача квартальных и годовых отчетов, представление интересов лесничества в Главном управлении лесами Челябинской области</li>
                <li>обеспечил высокие показатели работы по лесовосстановлению за время работы</li>
                <li>вывел лесной питомник ЧОБУ "Красноармейское лесничество" из второй десятки на уровень одного из лучших в Челябинской области</li>
              </ul>
            </td>
          </tr>
          <tr>
            <td>Апрель 2012 — январь 2018</td>
            <td>ФБУ "Российский центр защиты леса" - "Центр защиты леса Челябинской области", Челябинск<br>
            <b>инженер информационно-аналитического отдела</b><br>
              <ul>
                <li>осуществление государственного лесопатологического мониторинга</li>
                <li>ведение отчетности по защите леса и участие в составлении обзоров санитарного и лесопатологического состояния лесов</li>
                <li>ведение страницы организации на сайте rcfh.ru</li>
                <li>организация работы со СМИ и смежными организациями</li>
                <li>обеспечил высокие показатели в работе по государственному лесопатологическому мониторингу</li>
                <li>обеспечивал высокие показатели работы филиала среди филиалов ФБУ "Рослесозащита" по работе со СМИ и ведению сайта</li>
                <li>создал энтомологический музей Центра защиты леса Челябинской области</li>
              </ul>
            </td>
          </tr>
        </table>
        </div>
        <vueFooter />
  </div>
</template>

<script>
import vueFooter from '@/components/vueFooter'
export default {
name: 'work',
components: {
    vueFooter
  },
  data() { return {
    isActive: false,
    
   }
  }
}
</script>

<style scoped>
  
.work {
  background: #f8ffe8; /* Old browsers */
  background: -moz-radial-gradient(center, ellipse cover,  #f8ffe8 50%, #e3f5ab 100%, #b7df2d 100%); /* FF3.6-15 */
  background: -webkit-radial-gradient(center, ellipse cover,  #f8ffe8 50%,#e3f5ab 100%,#b7df2d 100%); /* Chrome10-25,Safari5.1-6 */
  background: radial-gradient(ellipse at center,  #f8ffe8 50%,#e3f5ab 100%,#b7df2d 100%); /* W3C, IE10+, FF16+, Chrome26+, Opera12+, Safari7+ */
  filter: progid:DXImageTransform.Microsoft.gradient( startColorstr='#f8ffe8', endColorstr='#b7df2d',GradientType=1 ); /* IE6-9 fallback on horizontal gradient */
}

.darkTheme {
  background: #253304; /* Old browsers */
  background: -moz-radial-gradient(center, ellipse cover,  #253304 50%, #e3f5ab 100%, #b7df2d 100%); /* FF3.6-15 */
  background: -webkit-radial-gradient(center, ellipse cover,  #253304 50%,#e3f5ab 100%,#b7df2d 100%); /* Chrome10-25,Safari5.1-6 */
  background: radial-gradient(ellipse at center,  #253304 50%,#e3f5ab 100%,#b7df2d 100%); /* W3C, IE10+, FF16+, Chrome26+, Opera12+, Safari7+ */
  filter: progid:DXImageTransform.Microsoft.gradient( startColorstr='#f8ffe8', endColorstr='#b7df2d',GradientType=1 ); /* IE6-9 fallback on horizontal gradient */
}

td {
  text-align: left;
}

table {
  padding-bottom: 10em;
}

.container {
  max-width: 960px;
  margin: 0 auto; 
}

h1 {
  margin: 0;
  padding: 0;
  padding-top: 2em;
  padding-bottom: 0.7em;
}

</style>