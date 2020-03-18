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

* Properties use dot operator (like .length)
* Methods also use dot operator but with paranthesis like .trim() or .toUpperCase()
* Built-in objects, including Math, are collections of methods and properties that JavaScript provides.
* Code not inside a function is GLOBAL.

[Cheat Sheet Javascript](https://www.codecademy.com/learn/introduction-to-javascript/modules/learn-javascript-introduction/cheatsheet)

[Javascript W3 Tutorials/Exercises](https://www.w3schools.com/js/exercise_js.asp?filename=exercise_js_variables1)

[Introduction cheat sheet](https://www.codecademy.com/learn/introduction-to-javascript/modules/learn-javascript-introduction/cheatsheet)
* Console.log()  
* Javascript  
* Methods  
* Libraries  
* Numbers  
* Strong.length  
* Data Instances  
* Booleans  
* Math.random()  
* Math.floor()  
* Single Line Comments  
* Null  
* Strings  
* Arithmetic Operators  
* Multi-line Comments  
* Assignment Operators  
* String Interpolation  
* Variables  
* Undefined  
* Declaring Variables  
* Template Literals  
* **let** keyword  
* **const** keyword  
* String Concatenation  

[Scope](https://www.codecademy.com/learn/introduction-to-javascript/modules/learn-javascript-scope/cheatsheet)
* Scope  
* Block Scoped Variables  
* Global Variables  

[Conditionals cheat sheet](https://www.codecademy.com/learn/introduction-to-javascript/modules/learn-javascript-control-flow/cheatsheet)
* Control Flow  
* Logical Operator OR **||**  
* Ternary Operator  
* Else Statement  
* AND **&&** Operator  
* Switch Statement  
* If Statement  
* Strict Comparisons  
* NOT **!** Operator  
* Comparison Operators  
* **if else, else if** Statement  
* Truthy and Falsy  


[Function cheat sheet](https://www.codecademy.com/learn/introduction-to-javascript/modules/learn-javascript-functions/cheatsheet)
* Arrow Functions (ES6)  
* Functions  
* Anonymous Functions  
* Function Expressions  
* Function Parameters  
* **return** Keyword  
* Function Declaration  
* Calling Functions  




> function **getGreeting**()  
* getGreeting is the function identifier and calling the code involves () parantheses.  
<img src="https://s3.amazonaws.com/codecademy-content/courses/learn-javascript-functions/Diagram/function+execution.svg">

# Function Expressions
    const plantNeedsWater = function(day)
    {
    if (day === 'Wednesday') {
    return true;
    }
    else {
        return false
        }
    }
    
# Parameters
<img src="https://s3.amazonaws.com/codecademy-content/courses/learn-javascript-functions/Diagram/function+parameters.svg">

# Arguments
    function sayThanks(name) {
    console.log('Thank you for your purchase ' + name + '! We appreciate your business.');
    }
    sayThanks('Cole');      
<img src="https://s3.amazonaws.com/codecademy-content/courses/learn-javascript-functions/Diagram/by_variable.svg">
* Outside of the curly braces, the function sayThanks is **called** and an **argument** (value) is put in there.

# Parameters
<img src="https://s3.amazonaws.com/codecademy-content/courses/learn-javascript-functions/Diagram/parameters.svg

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
    
  const plantNeedsWater = (day) => {
  return day === 'Wednesday' ? true : false;
};

VS

const plantNeedsWater = day => day === 'Wednesday' ? true : false;


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

# Other examples
    const logVisibleLightWaves = () => {
      let lightWaves = 'Moonlight';
        let region = 'The Arctic';
      // Add if statement here:
      if (region === 'The Arctic'){
        let lightWaves ='Northern Lights';
        console.log(lightWaves);
      }
      console.log(lightWaves);
    };

    logVisibleLightWaves();

# 1
    const famousSayings = ['Fortune favors the brave.', 'A joke is a very serious thing.', 'Where there is love there is life.'];

    let listItem = famousSayings[0];
    console.log(listItem);
    console.log(famousSayings[2]);
# 2
    let condiments = ['Ketchup', 'Mustard', 'Soy Sauce', 'Sriracha'];

    const utensils = ['Fork', 'Knife', 'Chopsticks', 'Spork'];

    condiments[0] = 'Mayo';
    console.log(condiments);

    condiments = ['Mayo'];
    console.log(condiments);

    utensils[3] = 'Spoon';
    console.log(utensils);
# 3
    const concept = ['arrays', 'can', 'be', 'mutated'];

    function changeArrt(arrt){
      arrt[3] = 'MUTATED';

    }


    changeArrt(concept);
    console.log(concept);

    function removeElement(newArr) {
      newArr.pop();
    }
    removeElement(concept);
    console.log(concept);
# 4
    let numberClusters = [[1,2],[3,4],[5,6]]

    const target = numberClusters[2][1];
    console.log(target)

# When to use WHILE loops VS FOR loops

So you may be wondering when to use a while loop! The syntax of a for loop is ideal when we know how many times the loop should run, but we don’t always know this in advance.   

Think of eating like a while loop: when you start taking bites, you don’t know the exact number you’ll need to become full. Rather you’ll eat while you’re hungry.  

In situations when we want a loop to execute an undetermined number of times, while loops are the best choice.

[forEach loop](https://www.youtube.com/watch?v=upP06o5ZPls)  
# forEach loop
    const fruits = ['mango', 'papaya', 'pineapple', 'apple'];  
    // Iterate over fruits below
    fruits.forEach(function (fruit, index) {
    console.log(`I want to eat a ${index}`);
    })
    
# .map method
    const animals = ['Hen', 'elephant', 'llama', 'leopard', 'ostrich', 'Whale', 'octopus', 'rabbit', 'lion', 'dog'];

    const secretMessage = animals.map(function (animal) {
      return animal[0];
    })

    console.log(secretMessage.join(''));
    
# 2nd .map method example
    
    const bigNumbers = [100,200,300,400,500];

    const smallNumbers = bigNumbers.map(function (numbo) {
      return numbo * 100;
      
    })
    console.log(smallNumbers);
    
# Concise body arrow Function vs Function Expression
    // CONCISE BODY ARROW FUNCTION
    const bigNumbers = [10,20,30].map(numbo => numbo * 200);

    // FUNCTION EXPRESSION
    const bigNumbers = [10,20,30].map(function(number) {
        return numbo * 200;
    });
# 3 different ways to .filter method
    const randomNumbers = [375, 200, 3.14, 7, 13, 852];

    // Call .filter() on randomNumbers below
    const smallNumbers = randomNumbers.filter(function(numbo) {
     if (numbo < 250) {
      return true;
     }
    }) ;
    console.log(smallNumbers)
    ----------------------------------
    const smallDumbers = randomNumbers.filter (function(dumbo) {
      return dumbo < 250;
    });
    console.log(smallDumbers);
    ----------------------------------
    const smallGumbers = randomNumbers.filter(gumbo =>
    gumbo < 250);
    console.log(smallGumbers);

# more .filter examples
        const favoriteWords = ['nostalgia', 'hyperbole', 'fervent', 'esoteric', 'serene'];

    const longFavoriteWords = favoriteWords.filter(skumbo =>        skumbo.length > 7);
    console.log(longFavoriteWords);
    --------------------------------------------
    const bongFavoriteWords = favoriteWords.filter(function(bungo) {
      return bungo.length > 7;
    });
    console.log(bongFavoriteWords);
