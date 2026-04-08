# Newtemat
/escape-room
main.js / main.py
gamestate.js
objects.js
inventory.js
interactions.js
const gameState = {
  inventory:[],
  drawerOpened: false,
  foundCode: false
}
const objects = {
  door: {
    locked; true
  },
  drawer: {
    opened: false,
    contains: "note"
  },
  painting: {
    clue: "1998"
  }
}
function addItem(key) {
  gameState.inventory.puch(key)
}

function hasItem(key) {
  return gameState.inventory.includes(key)
}
function interact(objectName) {
  if (objectName === "drawer") {
    gameState.drawerOpened) {
    addItem("note")
    console.log("Znalazłeś kartkę!") 
  } else {
  console.log("szuflada jest pusta")
  }
}
if (objectName === "painting") {
  console.log("Widzisz liczbę: 1998")
  gameState.foundCode = true
}

if (objectName === "door") {
  if (gameState.doorUnlocked) {
    console.log("Wygrałeś!")
  } else {
    console.log("Drzwi są zamknięte")
    }
  }
}
function enterCode(code) {
  if (code === "1998") {
    gameState.doorUnlocked = true
    console.log("Drzwi odblokowane!")
  } else {
    console.log("zły kod")
  }
}
console.log("Jesteś w pokoju. Znajdź sposób, żeby uciec. ")
// przykładowe akcje
interact("drawer")
interact("painting")
enterCode("1998")
interact("dorr")
