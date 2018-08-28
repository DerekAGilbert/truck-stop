<template>
  <div id='app'>
    <div id='app-body'>
      <div id="app-content">
        <router-view/>
      </div>
    </div>
  </div>
</template>

  <style lang="scss">
    #app,html,body {
    height: 100%;
    padding: 0px;
    margin: 0px;
    overflow:hidden;
    -webkit-overflow-scrolling: touch;
      #app-body {
        height:100%;
        display: flex;
        flex-direction: column;
        justify-content: center;
        overflow: auto;
        background: #141E30;  /* fallback for old browsers */
        background: -webkit-linear-gradient(to right, #243B55, #141E30);  /* Chrome 10-25, Safari 5.1-6 */
        background: linear-gradient(to right, #243B55, #141E30); /* W3C, IE 10+/ Edge, Firefox 16+, Chrome 26+, Opera 12+, Safari 7+ */

        #app-content {
          align-self: center;
        }
      }
    }
</style>
