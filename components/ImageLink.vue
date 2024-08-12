<template>
    <div>
      <a :href="link" target="_blank">
        <img :src="imageSrc" :alt="altText" class="image" />
      </a>
    </div>
  </template>
  
  <script>
  export default {
    props: {
      imageSrc: {
        type: String,
        required: true
      },
      link: {
        type: String,
        required: true
      },
      altText: {
        type: String,
        default: 'Image'
      }
    }
  }
  </script>
  
  <style scoped>
  .image {
    width: 100%;
    max-width: 500px;
    cursor: pointer;
  }
  </style>
  