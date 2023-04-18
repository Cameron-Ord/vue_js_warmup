<template>
  <div>
    <header class="Header"><page-header></page-header></header>
    <main class="Main">
      <section class="section_main">
        <article class="article_main">
          <page-main></page-main>
        </article>
        <article class="article_items">
          <menu-items></menu-items>
        </article>
      </section>
    </main>
    <footer class="Footer"><page-footer></page-footer></footer>

  </div>
</template>

<script>
import PageMain from './components/PageMain.vue';
import MenuItems from './components/MenuItems.vue';
import PageHeader from './components/PageHeader.vue';
import PageFooter from './components/PageFooter.vue';
export default {
  name: 'App',
  components: {
MenuItems,

PageHeader,

PageFooter,

PageMain
  }
}
</script>

<style>

*{

  padding: 0px;
  margin: 0px;

}

body{

  background-color: #FAF9F9;
}

.Header{

  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  min-height: 10vh;

  text-align: center;

  justify-items: center;

  align-items: center;

  background-color: #FFD6BA;


}


.Main{

  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  min-height: 80vh;

  text-align: center;

  justify-items: center;

  align-items: center;

}

.Main>.section_main{

  display: grid;

  grid-template-rows: 1fr 1fr;

  text-align: center;

  justify-items: center;

  align-items: center;

}

.Footer{

  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  min-height: 10vh;

  text-align: center;

  justify-items: center;

  align-items: center;

  background-color: #FFD6BA;
}

</style>
