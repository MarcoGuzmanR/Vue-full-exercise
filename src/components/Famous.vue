<template>
  <div id='famous'>
    <h2>
      Trending Stories
      <strong>({{ famous.length }})</strong>
    </h2>
    <ul class='list-group'>
      <li v-for='story in famous' class='list-group-item'>
        {{ story.writer }} said "{{ story.plot }}".
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
      };
    },
    computed: {
      famous() {
        return this.stories.filter(story => story.upvotes > 50);
      },
    },
  };
</script>
