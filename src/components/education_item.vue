<template>
 <li>
    {{education_place.years}} <br />
    {{education_place.university}}<br />
    {{education_place.speciality}} <br />
    {{education_place.faculty}} <br />
    {{education_place.form}} 
     
 </li>
</template>

<script>
export default {
    props: {
        education_place: {
            type: Object,
            required: true
        }
    }
}
</script>

<style scoped>
  li {
      margin-bottom: 2em;
  }
</style>