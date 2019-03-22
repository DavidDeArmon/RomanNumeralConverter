function convertToRoman(num) {
  let newNum = num
  let decimals = [ 1000, 900, 500, 400, 100, 90, 50, 40, 10, 9, 5, 4, 1 ];
  let romanNumeral = [ 'M', 'CM', 'D', 'CD', 'C', 'XC', 'L', 'XL', 'X', 'IX', 'V', 'IV', 'I' ];
  let newRoman = ''
  for(let i = 0; i<decimals.length;i++){
   while(decimals[i] <= newNum){
     newRoman +=romanNumeral[i]
     newNum -= decimals[i]
   }
    
  }

  console.log(newRoman)
  console.log(newNum)
 return newRoman
}

convertToRoman(2);
