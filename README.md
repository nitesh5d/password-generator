# password-generator


const array = ['java', 'script', 'online', 'compiler', 'main'];

function getRandomNumber() {
    return Math.floor(Math.random() * array.length);
}

const firstPickedWord = array[getRandomNumber()];
const secondPickedWord = array[getRandomNumber()];

let encryptedFirstWord = "";
let encryptedSecondWord = "";

for (let i = 0; i < firstPickedWord.length; i++) {
  let letter = firstPickedWord[i];
  if (letter == 'a'){
      encryptedFirstWord = encryptedFirstWord + "@";
  }
  else if (letter == 'i'){
      encryptedFirstWord = encryptedFirstWord + "!";
  }
  else if (letter == 'e'){
      encryptedFirstWord = encryptedFirstWord + "3";
  }
  else if (letter == 'o'){
      encryptedFirstWord = encryptedFirstWord + "0";
  }
  else if (letter == 't'){
      encryptedFirstWord = encryptedFirstWord + "+";
  }
  else if (letter == 's'){
      encryptedFirstWord = encryptedFirstWord + "$";
  }
  else {
      encryptedFirstWord = encryptedFirstWord + letter;
  }
}

for (let i = 0; i < secondPickedWord.length; i++) {
  let letter = secondPickedWord[i];
  if (letter == 'a'){
      encryptedSecondWord = encryptedSecondWord + "@";
  }
  else if (letter == 'i'){
      encryptedSecondWord = encryptedSecondWord + "!";
  }
  else if (letter == 'e'){
      encryptedSecondWord = encryptedSecondWord + "3";
  }
  else if (letter == 'o'){
      encryptedSecondWord = encryptedSecondWord + "0";
  }
  else if (letter == 't'){
      encryptedSecondWord = encryptedSecondWord + "+";
  }
  else if (letter == 's'){
      encryptedSecondWord = encryptedSecondWord + "$";
  }
  else {
      encryptedSecondWord = encryptedSecondWord + letter;
  }
}

console.log(encryptedFirstWord + "-" + encryptedSecondWord);
// console.log(encryptedSecondWord);
