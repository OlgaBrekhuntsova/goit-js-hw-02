# goit-js-hw-02

-----TASK-1-----

A station for selling and repairing droids is ready to launch, the only thing
left is to write the software for the sales department. Declare a function
makeTransaction(quantity, pricePerDroid, customerCredits) that composes and
returns a message about purchasing repair droids.

It declares three parameters, whose values will be provided when the function is
called:

quantity — the number of ordered droids

pricePerDroid — the price of one droid

customerCredits — the amount of funds in the customer’s account

Extend the function as follows:

Declare a variable to store the total order amount (the total cost of all
ordered droids) and assign it an expression that calculates this value.

Add a check to see if the customer can pay for the order:

if the amount to be paid exceeds the number of credits in the customer’s
account, the function must return the string "Insufficient funds!"

otherwise, the function must return the string "You ordered <quantity> droids
worth <totalPrice> credits!", where <quantity> is the number of ordered droids,
and <totalPrice> is their total cost.

Take the code below and insert it after declaring your function to check if it
works correctly. The results of its execution will be displayed in the console.

console.log(makeTransaction(5, 3000, 23000)); // "You ordered 5 droids worth
15000 credits!" console.log(makeTransaction(3, 1000, 15000)); // "You ordered 3
droids worth 3000 credits!" console.log(makeTransaction(10, 5000, 8000)); //
"Insufficient funds!" console.log(makeTransaction(8, 2000, 10000)); //
"Insufficient funds!" console.log(makeTransaction(10, 500, 5000)); // "You
ordered 10 droids worth 5000 credits!"

-----TASK-2-----

Declare a function formatMessage(message, maxLength) that takes a string (the
parameter message) and checks its length according to the specified maximum
length (the parameter maxLength).

Extend the function so that:

If the length of the string is equal to or less than maxLength, the function
returns the original string unchanged.

If the length exceeds maxLength, the function trims the string to maxLength
characters, adds an ellipsis "..." at the end, and returns the trimmed version.

Take the code below and insert it after declaring your function to check if it
works correctly. The results of its execution will be displayed in the console.

console.log(formatMessage("Curabitur ligula sapien", 16)); // "Curabitur
ligula..." console.log(formatMessage("Curabitur ligula sapien", 23)); //
"Curabitur ligula sapien" console.log(formatMessage("Vestibulum facilisis purus
nec", 20)); // "Vestibulum facilisis..." console.log(formatMessage("Vestibulum
facilisis purus nec", 30)); // "Vestibulum facilisis purus nec"
console.log(formatMessage("Nunc sed turpis a felis in nunc fringilla", 15)); //
"Nunc sed turpis..." console.log(formatMessage("Nunc sed turpis a felis in nunc
fringilla", 41)); // "Nunc sed turpis a felis in nunc fringilla"

-----TASK-3-----

The function checkForSpam(message) takes a string (the parameter message),
checks it for forbidden words "spam" and "sale", and returns the result of the
check. The words in the string parameter message may be in any case, for example
SPAM or sAlE.

Extend the function so that:

If a forbidden word (spam or sale) is found, the function returns the boolean
true.

If the string does not contain forbidden words, the function returns the boolean
false.

Take the code below and insert it after declaring your function to check if it
works correctly. The results of its execution will be displayed in the console.

console.log(checkForSpam("Latest technology news")); // false
console.log(checkForSpam("JavaScript weekly newsletter")); // false
console.log(checkForSpam("Get best sale offers now!")); // true
console.log(checkForSpam("Amazing SalE, only tonight!")); // true
console.log(checkForSpam("Trust me, this is not a spam message")); // true
console.log(checkForSpam("Get rid of sPaM emails. Our book in on sale!")); //
true console.log(checkForSpam("[SPAM] How to earn fast money?")); // true

-----TASK-4-----

Declare a function getShippingCost(country) that should check the possibility of
delivering goods to the user’s country (the parameter country) and return a
message with the result. Be sure to use the switch statement.

The format of the returned string is: "Shipping to <country> will cost <price>
credits", where <country> and <price> must be replaced with the corresponding
values.

List of countries and shipping costs:

China — 100 credits

Chile — 250 credits

Australia — 170 credits

Jamaica — 120 credits

From the list, it is clear that delivery is not available everywhere. If the
specified country is not in the list, the function must return the string:
"Sorry, there is no delivery to your country".

Take the code below and insert it after declaring your function to check if it
works correctly. The results of its execution will be displayed in the console.
console.log(getShippingCost("Australia")); // "Shipping to Australia will cost
170 credits" console.log(getShippingCost("Germany")); // "Sorry, there is no
delivery to your country" console.log(getShippingCost("China")); // "Shipping to
China will cost 100 credits" console.log(getShippingCost("Chile")); // "Shipping
to Chile will cost 250 credits" console.log(getShippingCost("Jamaica")); //
"Shipping to Jamaica will cost 120 credits"
console.log(getShippingCost("Sweden")); // "Sorry, there is no delivery to your
country"
