<template>
  <template v-for="item in cards" :key="item.title">
     <div class="card w-1/4 border-2 my-5 ml-96 rounded-2xl">
      <div class="title font-bold text-2xl text-center font-barlow py-2">
        <h2 class="font-bold">{{item.title}}</h2>
      </div>
      <hr>
      <div class="content font-nunito p-2">
        <p>{{item.content}}</p>
      </div>
      <hr>
      <div class="text-right mt-4 mr-2 mb-2">
        <button class="border-2 border-none rounded-lg text-white bg-blue-400 py-1 px-5 font-mono text-lg">Edit</button>
      </div>
    </div>
  </template>
</template>

<script>

export default {
  name: 'App',
  data() {
    return {
      message: 'Hello Vue!',
      cards: [
        {
          title: 'Card 1',
          content: 'Lorem ipsum dolor sit, amet consectetur adipisicing elit. Mollitia temporibus corporis quaerat voluptatibus? Quas odio culpa corporis illum? Corrupti tenetur omnis, '
        },
        {
          title: 'Card 2',
          content: 'Lorem ipsum dolor sit, amet consectetur adipisicing elit. Mollitia temporibus corporis quaerat voluptatibus? Quas odio culpa corporis illum? Corrupti tenetur omnis, '
        },
        
      ]
    }
  },
}
</script>

<style src="./assets/tailwind.css">
  @import url('https://fonts.googleapis.com/css?family=Nunito:400,700&display=swap');
  @import url('https://fonts.googleapis.com/css2?family=Barlow:ital@1&family=PT+Sans&display=swap');
</style>