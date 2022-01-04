<template>
  <div class="grid-container">
    <div class="name">
      <div>LUKAS MAXIMILIAN</div>
      <div>MASOPUST</div>
    </div>
    <button class="button" id="button1">Research</button>
    <button class="button" id="button2">Curriculum Vitae</button>
    <button class="button" id="button3">Portfolio</button>
    <div class="line-container">
      <div class="line" id="line1" />
      <div class="line" id="line2" />
      <div class="line" id="line3" />
    </div>
    <div class="divider">■</div>
    <a href="https://github.com/lukasmaxim" class="link">GitHub</a>
    <a href="mailto:lmasopust@ucdavis.edu" class="link">l.masopust at me.com</a>
    <a href="https://github.com/lukasmaxim" class="link">GitHub</a>
  </div>
</template>

<script>
export default {
  name: "Header"
};
</script>

<style>
a {
    font-weight: 900;
}
.divider {
    grid-area: divider;
}
.grid-container {
  display: grid;
  grid-template-columns: 0.3fr 1fr 1fr 1fr 1fr 0.3fr;
  grid-template-areas:
    ". name button1 button2 button3 ."
    "line line line line line line"
    /* ". link divider link divider ."; */
}
.name {
  margin: auto;
  grid-area: name;
  font-size: 30pt;
  text-align: left;
}
.button {
  grid-area: button;
}
button {
  position: relative;
  left: 50%;
  height: fit-content;
  width: fit-content;
  padding: 1em;
  border: 0.15em solid #393939;
  border-radius: 0.3em;
  cursor: pointer;
  font-family: "roboto mono";
  font-weight: 500;
  color: #393939;
  justify-content: center;
}
#button1 {
  grid-area: button1;
}
#button2 {
  grid-area: button2;
}
#button3 {
  grid-area: button3;
}
.line-container {
    margin-top: 1em;
  grid-area: line;
  vertical-align: top;
  height: 10em;
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
.point-1 {
  grid-area: point-1;
}
.point-2 {
  grid-area: point-2;
}
.link {
    grid-area: link;
}

</style>
