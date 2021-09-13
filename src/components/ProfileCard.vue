<template>
  <main class='profile-card'>
    <header class='profile-card__header'>
      <slot name='avatar'></slot>
    </header>
    <section class='profile-card__details'>
      <h2 class='title regular-text'>
        {{ title }}
        <span class='age'>{{ age }}</span>
      </h2>
      <p class='city small-text'>
        {{ city }}
      </p>
    </section>
    <footer class='profile-card__footer'>
      <div class='followers'>
        <p class='bold-text'>
          {{ followers }}
        </p>
        <p class='tiny-text'>Followers</p>
      </div>
      <div class='likes'>
        <p class='bold-text'>
          {{ likes }}
        </p>
        <p class='tiny-text'>Likes</p>
      </div>
      <div class='photos'>
        <p class='bold-text'>
          {{ photos }}
        </p>
        <p class='tiny-text'>Photos</p>
      </div>
    </footer>
  </main>
</template>

<script>
export default {
  name: 'ProfileCard',
  props: {
    title: {
      type: String,
      default: ''
    },
    age: {
      type: String,
      default: ''
    },
    city: {
      type: String,
      default: ''
    },
    followers: {
      type: String,
      default: ''
    },
    likes: {
      type: String,
      default: ''
    },
    photos: {
      type: String,
      default: ''
    }
  }
};
</script>
