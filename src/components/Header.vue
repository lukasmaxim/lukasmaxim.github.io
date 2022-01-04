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
  </div>
</template>

<script>
export default {
  name: "Header"
};
</script>

<style>
.grid-container {
  display: grid;
  grid-template-columns: 0.5fr 1fr 1fr 1fr 1fr 0.5fr;
  grid-template-areas:
    ". name button1 button2 button3 ."
    "line line line line line line";
}
.name {
  margin: auto;
  grid-area: name;
  font-size: 30pt;
  text-align: left;
}
button {
    height: 50px;
  border: 0.2em solid #D8D8D8;
  border-radius: 0.3em;
  cursor: pointer;
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
  grid-area: line;
  vertical-align: top;
  height: 10em;
}
.line {
  height: 1em;
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
.button {
  grid-area: button;
}
</style>
