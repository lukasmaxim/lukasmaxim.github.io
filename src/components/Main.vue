<template>
    <div class="grid-container">
        <div class="name">LUKAS MAXIMILIAN MASOPUST</div>
        <div class="lines">
            <img class="line" src="../assets/svgs/line1.svg" />
            <img class="line" src="../assets/svgs/line2.svg" />
            <img class="lines" src="../assets/svgs/line3.svg" />
        </div>
        <div class="subtitle subtitle-1">PhD Student</div>
        <div class="point1">
            <img src="../assets/svgs/circle.svg" width="20px"/>
        </div>
        <div class="subtitle subtitle-2">Retro Enthusiast</div>
        <div class="point2">
            <img src="../assets/svgs/circle.svg" width="20px"/>
        </div>
        <div class="subtitle subtitle-3">Cat Person</div>
        <div class="subtitle-4">VIDI @ UC DAVIS</div>
        <div class="buttons"></div>
    </div>
</template>

<script>
export default {
    name: "Main"
};
</script>

<style>
div {
}
.grid-container {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr 1fr 1fr;
    grid-template-areas:
    "name name name name name"
    "lines lines lines lines lines"
    "subtitle-1 point-1 subtitle-2 point-2 subtitle-3"
    "subtitle-4 subtitle-4 subtitle-4 subtitle-4 subtitle-4"
    "buttons buttons buttons buttons buttons";
}
.name {
    margin: auto;
    grid-area: name;
    font-size: 70pt;
}
.line {
    vertical-align:top;
}
.lines {
    grid-area: lines;
}
.point-1 {
    grid-area: point-1;
}
.point-2 {
    grid-area: point-2;
}
.subtitle {
    margin: auto;
    font-size: 30pt;
}
.subtitle-1 {
    grid-area: subtitle-1;
}
.subtitle-2 {
    grid-area: subtitle-2;
}
.subtitle-3 {
    grid-area: subtitle-3;
}
.subtitle-4 {
    margin: auto;
    grid-area: subtitle-4;
    font-size: 50pt;
}
.button {
    grid-area: button;
}
</style>