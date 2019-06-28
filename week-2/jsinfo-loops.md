> start (and try to finish) the [loop tasks](https://javascript.info/while-for) from javascript.info and paste each of your solutions into this file.  
> Don't be afraid of peeking at the solutions!  Just be sure you study them well

>1
let i = 3;

while (i) {
  alert( i-- );
}
SOLUTION:
let i = 3;

alert(i--); // shows 3, decreases i to 2

alert(i--) // shows 2, decreases i to 1

alert(i--) // shows 1, decreases i to 0

// done, while(i) check stops the loop

>2

>The prefix form ++i:

let i = 0;
while (++i < 5) alert( i );

>The postfix form i++

let i = 0;
while (i++ < 5) alert( i );
SOLUTION:
