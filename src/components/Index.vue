<template>
  <main>
    <section id="frame">
      <video id="looper" poster="https://s3-eu-west-1.amazonaws.com/echo-short-film/Pictureofsomething_1.1.1.jpg" muted autoplay loop>
        <source src="https://s3-eu-west-1.amazonaws.com/echo-short-film/Looper2.mp4">
      </video>
    </section>
    <section id="content"> 
      <menu>
        <h3>Coming May 2018</h3>
      </menu>
      <article id="title">
        <h1>
          Echo
          <img src="/static/battenberg-svg.svg">
        </h1>
      </article>
      <article id="footer">
        <p class="credits-block">
          TropeMachine
          <span class="title">presents an</span>
          Alex Hall
          <span class="title">film</span>
          "Echo"
          <span class="title">Written By</span>
          Peter Moulding,
          Alex Hall,
          <span class="title">story</span>
          Mikey Bailey,
          <span class="title">and</span>
          Matthew Clark
        </p>
        <p class="credits-block">
          <span class="title">Staring</span>
          Hayden Scott
          <span class="title">as "Tommy"</span>
          Luca Molinari
          <span class="title">as "Oscar"</span>
          Nicole Jennings
          <span class="title">as "India"</span>
          <span class="title">with</span>
          Matthew Robinson,
          Dennis Jones
          <span class="title">and</span>
          Josephine Jones
        </p>
        <p class="credits-block">
          <span class="title">Screenplay By</span>
          Alex Hall
          <span class="title">DoP</span>
          Mike Bailey
          <span class="title">Directed By</span>
          Ron Graves
        </p>
        <p>
          <a href="https://www.facebook.com/echo2018" target="_blank"><i class="fa fa-facebook"></i></a>
          <a href="https://www.instagram.com/echoshortfilm/" target="_blank"><i class="fa fa-instagram"></i></a>
        </p>
        <p class="legal-info">© TropeMachine 2018. All Rights Reserved.</p>
      </article>
    </section>
  </main>
</template>

<script>
export default {
  name: 'Index',
  data () {
    return {
      
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
* {
  color: rgba(255,255,255,0.66);
}
#frame {
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  overflow: hidden;
}

#looper {
  position: relative;
  object-fit: cover;
  object-position: 66% 33%;
  height: 100%;
  width: 100%;
}

#content {
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  align-items: stretch;
}

menu {
  margin: 0;
  padding: 1rem;
  min-height: 80px;
  background: linear-gradient(to bottom, rgba(1, 6, 27, 0.45) -10%,rgba(1, 6, 27,0) 100%);
}

header h3 {
  text-align: center;
}

#footer {
  background: linear-gradient(to bottom, rgba(1, 6, 27,0) 0%,rgba(1, 6, 27,0.75) 100%);
}

#footer a {
  margin-right: 2em;
  font-size: 1.2em;
}

#footer a:last-of-type {
  margin-right: 0em;
}

i:hover {
  color: rgb(123, 235, 255, 1);
}

a:hover {
  color: rgb(123, 235, 255);
}

#title {
  text-align: center;
}

#title h1 {
  font-size: 12vw;
  margin: 0.2em 0;
  text-transform: uppercase;
  color: rgba(255, 255, 255, 0.33);
  display: inline-block;
  text-align: center;
}

#title h1 img {
  width: 100%;
  display: block;
}

.legal-info {
  font-size: smaller;
}

.credits-block {
  font-family: 'Six Caps', sans-serif;
  margin: 0.01rem;
  font-size: 1.4em;
  text-transform: uppercase;
}

.credits-block span.title {
  font-size: 0.5em;
}

@media (min-width: 944px) {
  #content menu, #title, #footer {
    padding-left: 33vw;
  }
}
</style>
