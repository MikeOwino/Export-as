# Export-as

Named exports also conveniently offer a way to change the name of variables when we export or import them. We can do this with the as keyword.

Let’s see how this works. In our menu.js example

let specialty = '';
let isVegetarian = function() {
}; 
let isLowSodium = function() {
}; 
 
export { specialty as chefsSpecial, isVegetarian as isVeg, isLowSodium };
In the above example, take a look at the export statement at the bottom of the file.

The as keyword allows us to give a variable name an alias as demonstrated in specialty as chefsSpecial and isVegetarian as isVeg.
Since we did not give isLowSodium an alias, it will maintain its original name.

### QQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQ


1.
Remove the keyword export in front of each variable name, since we will no longer need it.


Hint
As an example

export function meetsStaffRequirements(availableStaff, requiredStaff) {
 ...
};
would just be written as

function meetsStaffRequirements(availableStaff, requiredStaff) {
 ...
};
2.
Add an export statement to export the availableAirplanes object as aircrafts, flightRequirements as flightReqs, the meetsStaffRequirements method as meetsStaffReqs and meetsSpeedRangeRequirements as meetsSpeedRangeReqs.


Hint
export { availableAirplanes as aircrafts, flightRequirements as flightReqs, meetsStaffRequirements as meetsStaffReqs, meetsSpeedRangeRequirements as meetsSpeedRangeReqs };
