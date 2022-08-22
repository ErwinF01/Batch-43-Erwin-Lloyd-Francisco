<template>
<q-toolbar class="bg-primary text-white">
      <q-btn flat round dense icon="menu" class="q-mr-sm" />
      <q-avatar>
        <img src="https://img.freepik.com/free-icon/todo-list_318-10185.jpg">
      </q-avatar>

      <q-toolbar-title>Wiwit inuman Piyesta</q-toolbar-title>

      <q-btn flat round dense icon="whatshot" />
    </q-toolbar>
  <q-input filled modelValue="" label="Filled" />
  <q-list bordered separator>
      <q-item clickable v-ripple :active="active">
        <q-item-section avatar>
          <input type="checkbox" />
        </q-item-section>
        <q-item-section> Iinom </q-item-section>
        <q-btn outline color="black" label="Delete" />
      </q-item>
        <q-item clickable v-ripple :active="active">
        <q-item-section avatar>
          <input type="checkbox" />
        </q-item-section>
        <q-item-section> Hindi Iinom</q-item-section>
       <q-btn outline color="black" label="Delete" />
      </q-item>
  </q-list>
     <q-btn-group push>
          <q-btn outline color="black" label="All" />
         <q-btn outline color="black" label="Active" />
         <q-btn outline color="black" label="Completed" />
    </q-btn-group>
<ul>
<!-- <li>
    <input type="checkbox" />
    asdasd
    <button> x </button>
</li>
<li>
 <input type="checkbox" />
    asdasd
    <button> x </button>   
</li>
<li>
    <input type="checkbox" />
    asdasda
    <button>x</button>
</li> -->
</ul>
<div class="q-pa-md">
    <div class="q-gutter-md row items-start">
      <q-img
        v-for="mode in fitModes"
        :key="mode"
        src="https://placeimg.com/500/300/nature"
        style="max-width: 300px; height: 150px;"
        :fit="mode"
      >
        <div class="absolute-bottom text-subtitle1 text-center">
          {{ mode }}
        </div>
      </q-img>
    </div>
  </div>
</template>
<style>
.h1{
    width: 200px;
    height: 100px;
    padding: 20px;
    border: 1px solid darkorange;
    border-radius: 8px;
  }
h1 {
    color: blue;
}
.title{
    color: pink;
}
#title{
    color: red;
    background-color: orange;
}
.q-btn-group {
  position: absolute;
  right: 50%;
}
</style>
