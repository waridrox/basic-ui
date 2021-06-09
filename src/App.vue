<template>
  <div id="app">
      <md-card>
        <md-card-header>
            <div class="md-title">
            FLINT UI
            </div>
        </md-card-header>
        <md-card-content>
          <md-button class="md-raised md-primary" v-on:click="apiRoute_spec()">Spec </md-button>

          <md-button class="md-raised md-primary" v-on:click="apiRoute_help()">Help </md-button>

          <md-button class="md-raised md-primary" v-on:click="apiRoute_version()">Version </md-button>

          <md-button class="md-raised md-accent" v-on:click="apiRoute_point()">Point </md-button>

          <md-button class="md-raised md-accent" v-on:click="apiRoute_rothc()">RothC </md-button>

        </md-card-content>

                  <md-button class="md-raised md-accent" v-on:click="cancel_operation()">CANCEL </md-button>

        <md-card-content>

        </md-card-content>


      </md-card>

      <md-card>
        <md-card-header>
          <div class="md-title">{{title}}</div>
        </md-card-header>
      </md-card>
  </div>
</template>

<script>
export default {
  name: 'App',
  data: function() {
    return {
      title: "Displays the current execution" 
    }
  },
  methods: {
    apiRoute_spec: function() {
      this.title = "SPEC route invoked";
      return this.title;
    },
    apiRoute_help: function() {
      this.title = "HELP route invoked";
      return this.title;
    }, 
    apiRoute_version: function() {
      this.title = "VERSION route invoked";
      return this.title;
    }, 
    apiRoute_point: function() {
      this.title = "POINT route invoked";
      return this.title;
    }, 
    apiRoute_rothc: function() {
      this.title = "ROTHC route invoked";
      return this.title;
    }, 
    cancel_operation: function() {
      this.title = "Operation was cancelled";
      return this.title;
    }
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
