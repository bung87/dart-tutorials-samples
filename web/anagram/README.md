## Moving elements within the DOM tree
[tutorials link](https://www.dartlang.org/docs/tutorials/add-elements/#moving-elements )  

When the program starts, it creates one button element for each of seven randomly selected letters. The program adds each button to a DOM element—a simple `<div>` element identified by the CSS selector `letterpile`—with a call to letterpile.children.add().  

![Dart code populates the letter pile with buttons](./anagram-newletters.png)  

Each button element in the letter pile has a mouse click handler called moveLetter(). If the button is in the letterpile, the mouse click handler moves the button to the end of the word. If the button is in the word, the mouse click handler moves the button back to the letter pile.  

To move the button from the letter pile to the word or back, the code simply adds the button to a DOM element that is different from the button’s current parent. Because an element can have only one parent, adding the button to a different parent automatically removes it from its previous parent.  

![The mouse click handler adds the button to the word, thus moving it](./anagram-move.png)  

The `+=` operator is a compound assignment operator, which combines an operation (`+`) with an assignment.

The `scrabbleValues` variable is a [Map](https://api.dartlang.org/dart_core/Map.html)—a data structure that contains key/value pairs. Use the square bracket syntax to retrieve a value by its key and the `length` property to get the number of pairs it contains.  

