# ReGextask.js

const readline = require('readline');

const rl = readline.createInterface({
    input: process.stdin,
    output: process.stdout
});

// Function to validate different types of credit cards
function validateCreditCard(cardNumber) {
    const visa = /^4[0-9]{12}(?:[0-9]{3})?$/
    const masterCard = /^5[1-5][0-9]{14}$/
    const amex = /^3[47][0-9]{13}$/
    const discover = /^6(?:011|5[0-9]{2})[0-9]{12}$/
    
    if (visa.test(cardNumber)) {
        return "Visa Card!!"
    } else if (masterCard.test(cardNumber)) {
        return "Master Card!!";
    } else if (amex.test(cardNumber)) {
        return "Amex Card!!!";
    } else if (discover.test(cardNumber)) {
        return "Discover Card!!";
    } else {
        return "Invalid card ";
    }
}

// Test the function
const cardNumber = "4111111111111111"; // Example Visa card number
console.log(validateCreditCard(cardNumber));

const cardDetails = "5277945729928485"
console.log(validateCreditCard(cardDetails)); // Master Card

const cardNumber2 = "347467626828424"    // Ameerican card
console.log(validateCreditCard(cardNumber2));

function interactWithUser() {
    rl.question("Enter card number: ", (userInput) => {
        console.log(validateCreditCard(userInput)); // Passing userInput instead of cardNumber
        rl.close();
    });
}

// Call the interaction function
interactWithUser();
