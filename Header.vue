<template lang="pug">
.header
  Slidshow
  header
    h1 Cresta Design
    ul: li(v-for="item in items") {{ item.list }}
</template>
<script>
export default {
  data () {
    return {
      items: [
        { list: 'Concept' },
        { list: 'Service' },
        { list: 'Work' },
        { list: 'Contact' }
      ]
    }
  },
  computed: {
  },
  methods: {
  }
}
</script>
<style lang="stylus">
.header {
  position: relative;

  img {
    width: 100%;
  }

  header {
    width: 100%;
    display: flex;
    position: absolute;
    top: 0;
    left: 0;
    padding: 20px 120px;
    color: #ffffff;
    align-items: center;

    h1 {
      flex: 1;
    }

    ul {
      display: flex;
      list-style: none;
      justify-content: flex-end;

      li {
        margin-left: 20px;
      }
    }
  }
}
</style>