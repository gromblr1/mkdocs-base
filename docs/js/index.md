    <style>
    p {
    font-family: 'helvetica neue', helvetica, sans-serif;
    letter-spacing: 1px;
    text-transform: uppercase;
    text-align: center;
    border: 2px solid rgba(0,0,200,0.6);
    background: rgba(0,0,200,0.3);
    color: rgba(0,0,200,0.6);
    box-shadow: 1px 1px 2px rgba(0,0,200,0.4);
    border-radius: 10px;
    padding: 3px 10px;
    display: inline-block;
    cursor: pointer;
    }
    </style>

    <p>Player 1: Chris</p> 

    <script>
      const para = document.querySelector('p');

      para.addEventListener('click', updateName);

      function updateName() {
        let name = prompt('Enter a new name');
        para.textContent = 'Player 1: ' + name;
      }
    </script>
    
* <font color="blue">**querySelector**</blue> is called a METHOD that you can use on the *document object* ('p').  
> objectName.methodName()  
* <font color="red">**addEventlistener**</font> is a called a method.  
* **click** is an event handler (e.g. mousedown, focus,blur etc) [W3Schools HTML DOM Events](https://www.w3schools.com/jsref/dom_obj_event.asp).  

*Note: "**const**" is like **var** or **let** except it cannot be changed.*  
*Note 2: Reusable code blocks are called "**functions**".*  

*Properties use dot operator (like .length)
*Methods also use dot operator but with paranthesis like .trim() or .toUpperCase()
*Built-in objects, including Math, are collections of methods and properties that JavaScript provides.

[Cheat Sheet Javascript](https://www.codecademy.com/learn/introduction-to-javascript/modules/learn-javascript-introduction/cheatsheet)

$ If/Else Statements
    let isEric = true;
    if (true) {
    console.log('im ericson');
        }
    else {
    console.log('i aint ericson');
        }


    let isEric2 = true;
    let name = "Ericsonnnn"
    isEric ? console.log('im ericson') : console.log(`i aint ${name}`);

# Logical Operators
    let mood = 'sleepster';
    let trdLevel = 2;
    if (mood === 'sleepster' && trdLevel > 5){
        console.log('IM FUCKING TIRED');
        }
        else {
        console.log('im not sleepy hehe');  
        }
