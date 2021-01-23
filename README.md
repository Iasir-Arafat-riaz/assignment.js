# assignment.js

// Convert kilo Meter To Meter using function
function kilometerToMeter(kilometer) {

  var meter = kilometer * 1000;
  return meter
}
var korim = kilometerToMeter(12);
console.log(korim);



//  //Budget Calculator using function 

function budgetCalculator(watch, phone, laptop) {
  var total = (watch * 50) + (phone * 100) + (laptop * 500);
  return total;
}
var totalBudget = budgetCalculator(2, 3, 4);
console.log(totalBudget);




//   // Hotel cost calculation in using function

function hotelCost(stayTime) {
  var hotelRent = 0;
  if (stayTime <= 10) {
    var firstPartCost = stayTime * 100;

  } else if (stayTime <= 20) {
    var firstPartCost = 10 * 100;
    var nextDays = stayTime - 10;
    var secondPartCost = nextDays * 80;
    hotelRent = firstPartCost + secondPartCost;
  } else {
    var firstPartCost = 10 * 100;
    var secondPartCost = 10 * 80;
    var nextDays = stayTime - 20;
    var thirdPartCost = nextDays * 50;
    hotelRent = firstPartCost + secondPartCost + thirdPartCost;

  }
  return hotelRent;
}



//Mega Friend using function

var friendsCircle = ["riaz", "miraj", "siraj", "ali", "amzad", "mosharraf", "shikder", "sir solimullah"];
function megaFriend(friend) {
  var length = 0;

  for (var i = 0; i < friend.length; i++) {

    if (friend[i].length > length) {
      length = friend[i].length;
      var longest = friend[i];
    }
  }
  return longest;
}


console.log(megaFriend(friendsCircle));
