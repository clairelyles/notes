##Day 2 Notes
###11/18/14

### MDN is a great resource for coding Q's  
### Javascript!


* ctrl + k clears
* Comments	
	* // = single line
	* /* */ multi line
	* ```<!---->``` = cmnd + / = comments out
* Data Types:
	* Numbers = integers (whole #), float (decimal pt)
	* Boolean = T or F
	* String
* Variables
	* ```var file_name = "a data type";```
	* ```file_name = "data type"``` is a GLOBAL variable. **be weary**
* Arrays
	* 	within ['brackets', 1, 2, 3]
	* 	ex: ```var a = [1,2,3,'true','false']```
		* 	```a[a.length-1]``` returns true
* Object String
	* ```person = {firstName:'Claire',lastName:'Lyles',age:35};```
		* ```person.firstName;``` returns 'Claire'
	* They are like arrays except that data is not stored in any sorted order and keys do not have to numbered indexes.

###Methods to the maddness
* Length: ```a.length``` retruns the TRUE lenght of array
* Length vs. Value: the true length of the array is the actual number of items in the array. If you want to recall a specific item inthe array, it is indexed at 0...1...2...etc
* Push: ```a.push('new value');``` adds a new item to the end of the array. Can be string, function, etc...
* Pop: ```var myValue = a.pop();``` will remove the last item inthe array and assign it to the myValue variable.
* Shift: ```array_name.shift();``` will remove the first item of the array
* Unshift: ```array_name.unshift();```  puts it in the beginning of the array
* Split: (array s) ```s.split(' ');``` returns the string into ('') individual letters,  (' ') split by spaces, or ('i') to split by i's and *remove* i's.
* Substring: ```s.substring(A,B)``` returns the part of the string between items A and B.
* ParseFloat: maintains decimals ParseFloat(num)+45 = 46.6
* ParseInt: removes decimals ParseInt(num)+45 = 46
* Math.round();
* Math.random(); is a rando # gen
* Math.ceil(); if # is 0.001 or 0.6 will always round up to 1

###Exercise #1

**Problem 3**

* Given a string "a, b, c"
* We need an array, so we assigned the variable friendsArray and split it using ```friends.split(",");```
* Then sorted the new freindsArray using ```friends.sort(",");```
* Finally show it in the console

**Problem 4**

* concat combines two arrays together
* ```var ourFriends2 = myFriends.concat(yourFriends).sort();
console(ourFriends2);```
* good habit to list off formulas

**Problem 5**

* add +1 so that you are calling the true length of the array 
* ```var foodRank = foods.indexOf("Pho")+1;
console.log(foodRank);```

###Murder Mystery

* ctrl + D mutliple panes verticle
* ctrl + shift + d splits selected screen horiz
* cmd + option + arrow

**Crimescene**

* search clues within crimescene using ```grep CLUE crimescene```


**Annabel**

* we have Annabel's name, so go to ```people``` folder and grep her name
* ```grep Annabel people```
* make note of her address

**Streets**

* given her address & line number of interview, we can use cat to view the file, and head & tail to select which part of the interview is important to us
* ```head -n 40 Hart_Place | tail -1``` OR ```head -40 Hart_Place | tail -1```
* retreive interview #

**Interview**

* cat interviews to view the specific interview
* ```cat interview-######```
* Get information about the lic # begins with "L337" and ends in "9"

**Go to Vehicles**

* grep multiple items about the car
* ```grep L337 vehicles -A 5``` means 1) search for lic containing L337, and include the next following 5 lines AFTER (-A) to cross check suspects with
* OR
* ```grep L337 vehicles -A 5 | grep Honda -B 1 -A 4 | grep Blue -B 2 -A 3``` searches for lic, honda, blue

**Search for J Bower**

* go to people
* write ```grep Bowers memberships/AAA``` or ```grep Bowers memberships/*``` /* is a wild card... so it searches for Bowers within ALL the files in the memberships folder.


















	
	
	

