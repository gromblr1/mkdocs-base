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

[Javascript W3 Tutorials/Exercises](https://www.w3schools.com/js/exercise_js.asp?filename=exercise_js_variables1)

> function **getGreeting**()  
* getGreeting is the function identifier and calling the code involves () parantheses.  
<img src="https://s3.amazonaws.com/codecademy-content/courses/learn-javascript-functions/Diagram/function+execution.svg">

# Parameters
<img src="https://s3.amazonaws.com/codecademy-content/courses/learn-javascript-functions/Diagram/function+parameters.svg">

# Arguments
    function sayThanks(name) {
    console.log('Thank you for your purchase ' + name + '! We appreciate your business.');
    }
    sayThanks('Cole');      
<img src="https://s3.amazonaws.com/codecademy-content/courses/learn-javascript-functions/Diagram/by_variable.svg">
* Outside of the curly braces, the function sayThanks is **called** and an **argument** (value) is put in there.

# Default Parameters (interpolation in a function)
    function greeting (name = 'stranger') {
    console.log(`Yello, ${name}!`);
    }
    greeting ('Nike');
    greeting();
    
## Default Parameters example 2
    function makeShoppingList(item1 = 'milk', item2 = 'bread', item3 = 'eggs'){
    console.log(`Remember to buy ${item1}`);
    console.log(`Remember to buy ${item2}`);
    console.log(`Remember to buy ${item3}`);
    }
    makeShoppingList()
    
### Default Parameters principles
    function funtionName(parameter = 'Default Value', parameter2 = 100, parameter3  = true) {
    // Function body here
    }
    
# *return* keyword
    const numOfMonitors = monitorCount(5,4);
    function monitorCount(rows, columns) {
    return rows * columns;
    };
    console.log(numOfMonitors);

# If/Else Statements
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

# ELSE IFs

    let season = 'spring';

    if (season === 'spring') {
    console.log('It\'s spring! The trees are budding!');
    } else {
    console.log('Invalid season.');
    }

    let stopLight ='others';

    if (stopLight === 'red') {
    console.log('STOP.');
    } else if (stopLight === 'yellow') { console.log(`Slow down, itz ${stopLight}`);}
    else if (stopLight === 'green') {
    console.log(`slow tf down, itz ${stopLight}`);
         }
    else { console.log('i dunno tbh');}

# switch
    let athleteFinalPosition = 'third place';

    switch (athleteFinalPosition) {
    case 'first place':
        console.log('You get the gold medal!');
        break;
    case 'second place':
        console.log('You get the silver medal!');
        break;
    case 'third place':
        console.log('You get the bronze medal!');
        break;
    default:
        console.log('No medal awarded.');
        break;
    }

# Logical Operators
    let mood = 'sleepster';
    let trdLevel = 2;
    if (mood === 'sleepster' && trdLevel > 5){
        console.log('IM FUCKING TIRED');
        }
        else {
        console.log('im not sleepy hehe');  
        }
