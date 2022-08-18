Describe: pigLatin()
Test: "It will add 'way' to the end of words that begin with letter a."
Code: pigLatin("a");
Expected Output: "away" 

// test 1
const a = "a";
function pigLatin(a) {
    return a + "way";
};

Test: "It will add 'way' to the end of any vowel."
Code: 
const vowel = ["a","e","i","o","u"];
pigLatin(vowel);
Expected Output: vowel + "way"

Test: "It will add 'way' to the end of every word that begins with a vowel"
Code:
const vowel = ["a","e","i","o","u"]
const word = "user";
pigLatin(word);
Expected Output: word + "way"



 let retVal = [];
    let wordToArray = word.split('');
    for(let i = 0; i <=vowel.length; i += 1) {
        if (wordToArray[0] === vowel[i]) {
            let addWay = word.concat("way");
            retVal.push(addWay);
    }
};
  
