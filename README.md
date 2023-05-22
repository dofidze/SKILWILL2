დავალება პირველი
##
function replaceValue(string, valueToReplace, valueToReplaceWith) {
  let newString = "";

  for (let i = 0; i < string.length; i++) {
    if (string[i] === valueToReplace) {
      newString += valueToReplaceWith;
    } else {
      newString += string[i];
    }
  }

  return newString;
}
console.log(replaceValue(`kodala`, `d`, `k`));

 
დავალება მეორე
##
const capitalWords = (tyaosaniUpper) => {
  return tyaosaniUpper.map((word) =>
    word
      .split(`_`)
      .map((w) => w.toUpperCase())
      .join(` `)
  );
};

console.log(
  capitalWords([
    `mastansa_kaba_emosa`,
    `garetma_vepxvis_tyavisa`,
    `xelta_nachedi_matraxi`,
    `hqonda_usxosa_mklavzeda`,
  ])
);

დავალება მესამე
##
const sortUsersByAge = (users) => users.sort((a, b) => a.age - b.age);

const users = [
  { name: "Lasha", age: 30 },
  { name: "Saba", age: 20 },
  { name: "Nino", age: 25 },
];

const sortedUsers = sortUsersByAge(users);
console.log(sortedUsers);
