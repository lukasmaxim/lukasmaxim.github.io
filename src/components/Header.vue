<template>
  <div class="grid-container">
    <div id="name">
      <div>LUKAS MAXIMILIAN</div>
      <div>MASOPUST</div>
    </div>
    <div id="button-container">
      <router-link to="research" tag="button" id="button1"
        >Research</router-link
      >
      <router-link to="cv" tag="button" id="button2"
        >Curriculum Vitae</router-link
      >
      <router-link to="portfolio" tag="button" id="button3"
        >Portfolio</router-link
      >
    </div>
    <div id="line-container">
      <div class="line" id="line1" />
      <div class="line" id="line2" />
      <div class="line" id="line3" />
    </div>
    <div id="link-container">
      <a href="https://github.com/lukasmaxim" class="link" id="link1">GitHub</a>
      <div id="divider1">■</div>
      <a href="mailto:lmasopust@ucdavis.edu" class="link" id="link2"
        >l.masopust at me.com</a
      >
      <div id="divider2">■</div>
      <a href="https://github.com/lukasmaxim" class="link" id="link3">Alamy</a>
    </div>
  </div>
</template>

<script>
export default {
  name: "Header"
};
</script>

<style>
.grid-container {
  margin-top: 40px;
  display: grid;
  grid-template-columns: 0.3fr 1fr 1fr 1fr 1fr 1fr 0.3fr;
  grid-template-areas:
    ". name name buttons buttons buttons ."
    "line line line line line line line"
    ". . links links links . .";
}
#button-container {
  grid-area: buttons;
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 1.5em;
}
#name {
  font-family: Lovelo;
  margin: auto;
  grid-area: name;
  font-size: 30pt;
  text-align: left;
}
#line-container {
  margin: 1em 0 1em 0;
  grid-area: line;
  vertical-align: top;
}

.line {
  height: 0.7em;
}
#line1 {
  background-color: #f4ac0a;
}
#line2 {
  background-color: #e00138;
}
#line3 {
  background-color: #570d49;
}
#link-container {
  grid-area: links;
  display: flex;
  justify-content: space-around;
  margin-bottom: 1em;
}
</style>
