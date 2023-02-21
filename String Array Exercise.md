
  1. Count number of words in a Text after splitting it by any word 
 
    ```
    let word = "Hello Wecode Acacdemy";
    let wordSplit =word.split(" ");
    console.log(wordSplit,wordSplit.length);
    ```


 2. Convert odd position word to lowercase and even position word to uppercase
 Hello WeCode Academy 
 hello WECODE academy
```
 let str = "Hello WeCode Academy ";
 const words = str.split(' ');
 for (let i = 0; i < words.length; i++) {
   if (i % 2 === 0) {
     words[i] = words[i].toLowerCase();
   } else {
    words[i] = words[i].toUpperCase();
   }
}
 console.log(words);
```

 3 Capitalize each word of the string 
 hello wecode academy jhotwara jaipur 
 Hello Wecode Academy Jhotwara Jaipur 
```
 let str = "hello wecode academy jhotwara jaipur";
 let capitalizedStr = str.split(' ');
 console.log(capitalizedStr);
 for(let i =0;i<capitalizedStr.length;i++){
     capitalizedStr[i]=capitalizedStr[i][0].toUpperCase( )  + capitalizedStr[i].substring(1);
 }
 console.log(capitalizedStr)
```

 4. Convert an string into 2 halfs and change the position of the other half 
    My name is wecode academy
    wecode academy My name is 
```
 let strPosition ="My name is wecode academy";
 let strsplit = strPosition.slice(11);
 let secondstr =strPosition.slice(0,10);
 let strJoin =strsplit.concat(" " +secondstr ) ;
 console.log(strJoin.split(" "));
```

 6.Reverse a string 
```
 let strReverse =  "My name is wecode academy"
 let starr =strReverse.split("")
 console.log(starr.reverse().join().split(" "));
```

 7. Check string is palindrom or not
```
 let str = "helleh";
 let palindrom  = "";
 let strArr = str.split(" ");
  for (let i = strArr.length - 1; i >= 0; i--) {
     palindrom  = palindrom  + strArr[i];
 }
if (palindrom  === str) {
   console.log("Yes");
 } else {
   console.log("No");
 }
 console.log(palindrom.split(" ") )
```
8. Remove space from the string and show the output My name is wecode Mynameiswecode
```
  let str = "My name is wecode";
  let strspace = str.split(" ")
  console.log(strspace.join("").split(" "));
```
 10. Replace a word in string 
   My code is wecode and wecode Jhotwara, Jaipur.  
   code rodd
    My rodd is werodd and werodd Jhotwara, Jaipur
```
 let replaceStr=   "My code is wecode and wecode Jhotwara, Jaipur.";
 let newstr= replaceStr.replace(/code/g,"rodd");
 console.log(newstr)
