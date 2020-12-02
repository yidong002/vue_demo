<template>
  <div class="about">
    <h1>This is an about page</h1>
    <ul class="infinite-list" v-infinite-scroll="load" style="overflow:auto">
      <li v-for="i in count" :key="i" class="infinite-list-item">{{ i }}</li>
    </ul>
  </div>
</template>
<script>
export default {
  name: 'About',
  data () {
    return {
      count:10
    }
  },
  methods: {
    load () {
      // this.count += 10
    }
  }
}
</script>
