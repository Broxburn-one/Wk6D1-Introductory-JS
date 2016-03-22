//Section 1

//what types are these? Write your answer in a comment beside it.

1;				numeric
"cat";			string
true;			boolean
[];				array
{};				hash
1.1;			numeric
undefined;		undefined

//Section 2

// what is the truthy/falsiness values of the following
// write your answer in a comment beside it
// you can use an if to test this...
1; //true
"cat";      // true
true;       // true
NaN;        // false
[];			// true
{};			// true
undefined;	//false
"";			// false
0;			false


//Section 3

//Using examples that are different from above...

//3.1 Assign a variable that is a number		var num1 = 3;
//3.2 Assign a variable that is a string		var myName = "Fred";
//3.3 Assign a variable that is a boolean		var myBool = true;
//3.4 Assign a variable that is an object		var myArr = [];

//Section 4
//4.1 Write a statement that writes "hello" to the console if it's true and "bye" if it is false


var num1 = 1;
if ( num1 < 3) {
	console.log("Hello");
else
	console.log("bye");
end





//Section 5
var animals = ["raccoon","hedgehog","mouse","gerbil"];

//5.1. Assign the first element to a variable
//5.2. Assign the last element to a variable
//5.3. Assign the length of an array to a variable
//5.4. Add an item to the end of the array
//5.5. Add an item to the start of the array
//5.6. Assign the index of hedgehog to a variable


5.1   var elem1 = animals[0];
5.2   var elem2 = animals[animals.length-1];
5.3   var arrLen = animals.length;
5.4   animals.push("gazelle");
5.5   animals.unshift("rhino");
5.6   var hhIndex = animals.indexOf("hedgehog");





//Section 6

//6.1 Create an array of 5 vegetables
//6.2 Loop over the array and write to the console using a "while"
//6.3 Loop again using a "for" with a counter
//6.4 Loop again using a "for in"

6.1
var veggies = ["onions", "sprouts", "carrots", "beetroot", "cucumber"];

6.2
while (i < veggies.length) {
	console.log(veggies[i];
	i++;
}

6.3
for (x = 0; x < veggies.length; x++) {
	console.log(veggies[x]):
}

6.4
for ( var property	in veggies ) {
	console.log(veggies[property]);
}











//Section 7
var accounts = [
  { name: 'jay',
    amount: 125.50,
    type: 'personal'
  },
  { name: 'val',
    amount: 55125.10,
    type: 'business'
  },
  { name: 'marc',
    amount: 400.00,
    type: 'personal'
  },
  { name: 'keith',
    amount: 220.25,
    type: 'business'
  },
  { name: 'rick',
    amount: 1.00,
    type: 'personal'
  },
]
//7.1 Calculate the total cash in accounts
//7.2 Find the name of the account with the largest balance
//7.3 Find the name of the account with the smallest balance
//7.4 Calculate the average bank account value
//7.5 Find the value of marcs bank account
//7.6 Find the holder of the largest bank account
//7.7 Calculate the total cash in business accounts
//7.8 Find the largest personal account owner


7.1
var total = 0;
for (var property in accounts) {
  total += accounts[property].amount;
}
console.log(total);



7.2 Largest Balance

var largest = 0;
for (var property in accounts) {
   if ((accounts[property].amount) > largest) {
      largest = accounts[property].amount;
   } 
}
 console.log(largest);


7.3 Smallest Balance

var smallest = 0;
for (var property in accounts) {
   if ((accounts[property].amount) < smallest) {
      smallest = accounts[property].amount;
   } 
}
 console.log(largest);



7.4  Average Bank Account Value


var total = 0;
for (var property in accounts) {
  total += accounts[property].amount;
}
average = total / accounts.length;
console.log(average.toFixed(2));


7.5 Value of Marc's Bank Account

var markIndex = accounts.indexOf('marc');
marcBalance = accounts[markIndex].amount;


7.6 Holder of largest bank account

var largest = 0;
var holder = "";
for (var property in accounts) {
   if ((accounts[property].amount) > largest) {
      largest = accounts[property].amount;
      holder = accounts[property].name;
   } 
}
 console.log(holder);


7.7 Total Cash in Business Accounts

var total = 0;
for (var property in accounts) {
   if ((accounts[property].type) === "business") {
      total +=  = accounts[property].amount;
   } 
}
 console.log(total);


7.8 Largest Personal Account Owner

var largest = 0;
for (var property in accounts) {
  if (accounts[property].type == "personal") {
   if ((accounts[property].amount) > largest) {
      largest = accounts[property].amount;
      name = accounts[property].name;
    } 
  }
}
 console.log(name);







//Section 8
//Assign a variable myPerson to a hash, giving them a name, height favourate food

myPerson = {
  name: "Fred Bloggs",
  height: 1.80,
  favouriteFood: "crisps"
  }