<template>
  <div class="home">
    <img alt="Моя фотография" src="../assets/my_photo.jpg" width="300" height="300">
    <education
      v-bind:education_places="education_places"
     />
  </div>
</template>

<script>
  import education from '@/components/education'


export default {
  name: 'Home',
  data() {
    return {
      education_places: [
        {years: '2015-2017', speciality: 'Специальность: государственное и муниципальное управление', faculty: 'Факультет Управления', form: 'Заочная', university: 'ЧелГУ'},
        {years: '2003-2008', speciality: 'Специальность: биоэкология', faculty: 'Биологический факультет', form: 'Заочная', university: 'ЧелГУ'},
        {years: '1996-2008', university: 'Школа №1 г.Челябинска'}
      ]

    }
  },
  components: {
    education
  }
}
</script>

<style >
  img {
    border-radius: 50%;
    margin-top: 2em;
    margin-bottom: 2em;
  }

  .home {
    background: #f8ffe8; /* Old browsers */
    background: -moz-radial-gradient(center, ellipse cover,  #f8ffe8 50%, #e3f5ab 100%, #b7df2d 100%); /* FF3.6-15 */
    background: -webkit-radial-gradient(center, ellipse cover,  #f8ffe8 50%,#e3f5ab 100%,#b7df2d 100%); /* Chrome10-25,Safari5.1-6 */
    background: radial-gradient(ellipse at center,  #f8ffe8 50%,#e3f5ab 100%,#b7df2d 100%); /* W3C, IE10+, FF16+, Chrome26+, Opera12+, Safari7+ */
    filter: progid:DXImageTransform.Microsoft.gradient( startColorstr='#f8ffe8', endColorstr='#b7df2d',GradientType=1 ); /* IE6-9 fallback on horizontal gradient */
  }
</style>
