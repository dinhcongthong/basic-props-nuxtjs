<template>
  <div>
    <TestProps :user="userThong" @update-cart="updateCart2" />
  </div>

</template>

<script>
  import TestProps from '../components/TestProps.vue';
  export default {
    data (){
      return {
        userThong: 'Dinh Cong Thong'
      }
    },
    methods: {
      updateCart2 (e) {
        console.log(e);
      }
    },
    name: "IndexPage",
    components: { TestProps }
  }
</script>
