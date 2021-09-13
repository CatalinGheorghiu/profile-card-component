<template>
  <div id='app'>
    <ProfileCard age='26'
                 city='London'
                 followers='80K'
                 likes='803K'
                 photos='1.4K'
                 title='Victor Crest'>
      <template v-slot:avatar>
        <img :src='require(`@/images/image-victor.jpg`)' alt='Avatar' class='avatar'>
      </template>
    </ProfileCard>
  </div>
</template>

<script>

import ProfileCard from '@/components/ProfileCard.vue';

export default {
  name: 'App',
  components: {
    ProfileCard

  }
};
</script>

