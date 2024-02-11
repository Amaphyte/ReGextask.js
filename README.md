This code deals with the validation of various cards and how to determine the kind of card in use through the card number being inputted


const visa = /^4[0-9]{12}(?:[0-9]{3})?$/
    const masterCard = /^5[1-5][0-9]{14}$/
    const amex = /^3[47][0-9]{13}$/
    const discover = /^6(?:011|5[0-9]{2})[0-9]{12}$/
    
    The variables above are examples of cards we have and the regex codes is used to diffrentiate these cards so that when javascript matches the string and all conditions are met then it display the necessary results as intended

  visa cards starts with a digit 4 with any twelve digits ranging from 0 to 9 and another 3 digits from same range 0 to 9
(basically javascript with the help of regex pin points all cards starting with 4 as a digit to determine the card in use)

mastercard on the other hand has a starting digit of 5 after which are other conditions to be met indicating the card in use is a master

amex has its starting digit to be 3 while discover to be 6

In continuation to these regex function which was placed under a function, is the use of an if statement to make sure all conditions for determining the type of card in use are met 

lastly in the streams of code was a redline function giving an option for external users to key in their card number of which is then validated by javascript to ascertain the type of card in operation by the card numbeer inputted witht the help of the regex code 
