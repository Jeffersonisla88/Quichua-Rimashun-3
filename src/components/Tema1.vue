<template>
    <div class="phoneme-container">
      <h2>Kichwa Phonemes</h2>
      <div class="phoneme-group">
        <h3>Consonants</h3>
        <ul>
          <li v-for="phoneme in consonantPhonemes" :key="phoneme">{{ phoneme }}</li>
        </ul>
      </div>
      <div class="phoneme-group">
        <h3>Semiconsonants</h3>
        <ul>
          <li v-for="phoneme in semiconsonantPhonemes" :key="phoneme">{{ phoneme }}</li>
        </ul>
      </div>
      <div class="phoneme-group">
        <h3>Vowels</h3>
        <ul>
          <li v-for="phoneme in vowelPhonemes" :key="phoneme">{{ phoneme }}</li>
        </ul>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        consonantPhonemes: ['p', 't', 'k', '*q', 'č', 'h', 's', 'š', 'm', 'n', 'ñ', 'l', 'l y', 'r'],
        semiconsonantPhonemes: ['w', 'y'],
        vowelPhonemes: ['i', 'u', 'a']
      };
    }
  };
  </script>
  
  <style>
  .phoneme-container {
    /* Add your desired styling here */
  }
  .phoneme-group {
    /* Add your desired styling here */
  }
  </style>