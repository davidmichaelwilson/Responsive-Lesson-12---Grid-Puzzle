# Lesson plan
  
---

Answer:

```

/* Colors are black, red, green, yellow, blue, pink, gray, brown, orange and purple */

body, html {
  margin: 0;
  padding: 0;
  color: white;
}

.box {
  min-width: 62px;
  min-height: 150px;
}

div {
  border: solid black 1px;
}

#boxes {
  display: grid;
  grid-template-areas: 
    "One One   Two   Three Three" 
    "One One   Four  Five  Five"
    "Six Seven Seven Five  Five"
    "Six Eight Nine  Nine  Ten";
}




/* Edit below this line: */

#box1 {
  background-color: white;
  color: black;
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  grid-template-rows: 150px;
  grid-area: One;
}

#box1item2 {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  grid-template-rows: 75px;
  align-items: center;
  justify-items: center;
}

#box2 {
  background-color: red;
  display: flex;
  justify-content: end;
  align-items: end;
  grid-area: Two;
}

#box3 {
  background-color: green;
  display: flex;
  text-align: center;
  align-items: center;
  grid-area: Three;
}

#box3 > div {
  flex: 1;
}

#box4 {
  background-color: yellow;
  color: black;
  display: flex;
  align-items: center;
  grid-area: Four;
}

#box5 {
  background-color: blue;
  display: grid;
  grid-template-areas: 
    "TopLeft Right"
    "BotLeft Right";
  grid-template-columns: repeat(2, 1fr);
  grid-area: Five;
}

#box5item1 {
  grid-area: TopLeft;
  display: flex;
  justify-content: center;
}

#box5item2 {
  grid-area: Right;
  display: flex;
  flex-direction: column;
}

#box5item2 > div {
  flex: 1;
  display: flex;
  justify-content: center;
  align-items: center;
}

#box5item3 {
  grid-area: BotLeft;
  display: flex;
  justify-content: end;
}


#box6 {
  background-color: pink;
  display: flex;
  flex-direction: column;
  grid-area: Six;
}

#box6 > div {
  flex: 1;
  display: flex;
  align-items: center;
}

#box7 {
  background-color: gray;
  grid-area: Seven;
  display: flex;
  justify-content: end;
  align-items: center;
}

#box8 {
  background-color: brown;
  display: flex;
  align-items: end;
  justify-content: center;
  grid-area: Eight;
}

#box9 {
  background-color: orange;
  display: flex;
  grid-area: Nine;
}

#box9 > div {
  flex: 1;
  display: flex;
  align-items: center;
}

#box9 :first-child {
  justify-content: end;
}

#box10 {
  background-color: purple;
  grid-area: Ten;
  display: flex;
  align-items: center;
  justify-content: center;
}

```