<template>
  <div class='container'>
    <ul class='list-group'>
      <li class='list-group-item' v-for='story in stories' :key='story'>
        {{ story.writer }} said "{{ story.plot }}"
        Story upvotes {{ story.upvotes }}.
      </li>
    </ul>
  </div>
</template>

<script>
  import store from '../store';

  export default {
    data() {
      return {
        stories: store.stories,
      }
    },
    created() {
      console.log('stories');
    },
  };
</script>
