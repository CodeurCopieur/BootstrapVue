<template lang="pug">
  #app
    b-container.bv-example-row
      b-row
        b-col(cols="4") cols="4" eius explicabo unde in dicta, vero repellendus et! Blanditiis incidunt unde quibusdam magnam, natus corporis consequatur voluptatibus molestias hic qui cumque.</b-col>
        b-col(cols="4") cols="4" Lorem ipsum dolor sit amet consectetur adipisicing elit. Assumenda iusto sit quibusdam magni, et aut inventore? Provident nisi dolores impedit consequatur dolor, quam nihil debitis totam adipisci quibusdam doloremque aliquam.</b-col>
        b-col(cols="4") cols="4" Lorem, ipsum dolor sit amet consectetur adipisicing elit. Asperiores adipisci similique ad rerum!</b-col>

      hr

      b-row
        b-col(md="4") md="4" eius explicabo unde in dicta, vero repellendus et! Blanditiis incidunt unde quibusdam magnam, natus corporis consequatur voluptatibus molestias hic qui cumque.</b-col>
        b-col(md="4") md="4" Lorem ipsum dolor sit amet consectetur adipisicing elit. Assumenda iusto sit quibusdam magni, et aut inventore? Provident nisi dolores impedit consequatur dolor, quam nihil debitis totam adipisci quibusdam doloremque aliquam.</b-col>
        b-col(md="4") md="4" Lorem, ipsum dolor sit amet consectetur adipisicing elit. Asperiores adipisci similique ad rerum!</b-col>

      hr

      b-row
        b-col(md="4") cols="4" Lorem ipsum, dolor sit amet consectetur adipisicing elit. Dolor, laborum? Est omnis facilis id consectetur eveniet dignissimos, deserunt iste quibusdam enim alias, veniam pariatur velit placeat, perspiciatis eius exercitationem eos.
        b-col(md="4" offset-md="4") md="4" offset-md="4" Lorem ipsum dolor sit amet consectetur adipisicing elit. Distinctio provident quo amet voluptate obcaecati earum vero eaque sequi voluptates quaerat culpa tempora suscipit blanditiis quis repellat, voluptatem optio. Error, a.
      
      hr

      b-row(align-v="center").test-height
        b-col Lorem ipsum dolor sit amet.
        b-col Lorem ipsum dolor sit amet.
        b-col Lorem ipsum dolor sit amet.
        
      hr

      b-row(align-h="center").test-height
          b-col(cols="4")
            b-button(size="lg" variant="success" @click="handleClick") Mon Bouton
          b-col(cols="4") Lorem ipsum dolor sit amet.

      hr

      b-row(align-v="center" align-h="center").test-height
          b-col(cols="4")
            b-button(size="lg" variant="success"  @click="handleShow") Mon Bouton
          b-col(cols="4") 
            b-alert(variant="danger" dismissible :show="showDismissibleAlert" @dismissed="showDismissibleAlert").mb-0 Dismissible Alert!
      
      

</template>

<script>

export default {
  name: 'App',
  data() {
    return {
      showDismissibleAlert: false
    }
  },
  methods: {
    handleClick() {
      console.log('test mon bouton');
    },
    handleShow() {
      this.showDismissibleAlert = true
    }
  }
}
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

.test-height {
  height: 10rem;
  background-color: rgba(255,0,0,.1);
}
</style>
