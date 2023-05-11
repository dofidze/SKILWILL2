დავალება პირველი

function findUserWithMinimumAge(users) {
  const userWithMinimumAge = users.reduce((prev, current) => {
    return prev.age < current.age ? prev : current;
  });

  return userWithMinimumAge.name;
}

let users = [
  { name: "Temo", age: 25 },
  { name: "Lasha", age: 29 },
  { name: "Ana", age: 28 },
];
const result = findUserWithMinimumAge(users);
console.log(result);



დავალება მეორე


let users = [
  { name: "Temo", age: 25 },
  { name: "Lasha", age: 29 },
  { name: "Ana", age: 28 },
];
const result = findUserWithMinimumAge(users);
console.log(result);

let user = {
  name: "tommy jerry",
  age: 30,
  email: "tommyjerry@gmail.com",
  address: "Georgia tbilisi St.221",
};

function getSignificantValues(user) {
  return {
    name: user.name,
    age: user.age,
    email: user.email,
    address: user.address,
  };
}

let significantValues = getSignificantValues(user);

console.log(significantValues);


დავალება მესამე

let aTries = 1;
let bTries = 1;

while (true) {
  let aRoll = Math.floor(Math.random() * 6) + 1;
  aTries++;
  if (aRoll === 3) {
    console.log("Customer a wins in " + aTries + " tries!");
    break;
  }

  let bRoll = Math.floor(Math.random() * 6) + 1;
  if (bRoll === 3) {
    console.log("Customer b wins in " + bTries + " tries!");
    break;
  }
}

function maxAge(users) {
  return users.reduce((max, person) => {
    return person.age > max ? person.age : max;
  }, 0);
}

let users = [
  { name: "Temo", age: 25 },
  { name: "Lasha", age: 29 },
  { name: "Ana", age: 28 },
];
maxAge(users);
console.log(maxAge(users));
