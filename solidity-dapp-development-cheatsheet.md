## Solidity Cheat Sheet:

### Data Types:

- uint: unsigned integer (0 to 2^256 - 1)
- int: signed integer (-2^255 to 2^255 - 1)
- bool: boolean (true or false)
- address: address of an Ethereum account
- string: sequence of UTF-8 characters
- bytes: sequence of bytes
- fixed/ufixed: fixed-point decimal

### Variables:

- Declared using data type, followed by variable name. Example: uint age;
- Variables can be initialized during declaration, Example: uint age = 25;
- Variables are private by default and can be made public using the "public" keyword.

### Functions:

- Declared using the "function" keyword, followed by function name and parameters within parentheses. Example: function setAge(uint newAge) {}
- Can return a value using the "return" keyword.
- Functions can be called using the function name and passing the required parameters. Example: setAge(30);

### Events:

- Declared using the "event" keyword, followed by event name and parameters within parentheses. Example: event NewAgeSet(uint newAge);
- Triggered using the "emit" keyword. Example: emit NewAgeSet(newAge);

### Modifiers:

- Used to modify the behavior of functions.
- Declared using the "modifier" keyword, followed by modifier name and code within curly braces. Example: modifier onlyOwner { if (msg.sender != owner) throw; \_; }
- Applied to functions using the "modifier" keyword followed by the modifier name. Example: function setAge(uint newAge) public onlyOwner { ... }

### Mapping:

- Used to store key-value pairs.
- Declared using the "mapping" keyword, followed by the data type of the key and value within square brackets. Example: mapping(address =\> uint) balances;

### Structs:

- Used to store multiple values of different data types.
- Declared using the "struct" keyword, followed by the struct name and variables within curly braces. Example: struct Person { uint age; string name; }

### Arrays:

- Used to store a collection of values of the same data type.
- Declared using the data type, followed by the variable name within square brackets. Example: uint[] ages;

### Operators:

- Arithmetic: +, -, \*, /, %
- Comparison: ==, !=, \>, \<, \>=, \<=
- Logical: &&, ||, !

## Get Started with DApp Development:

1. Set up your development environment: Install a local blockchain platform like Ganache or use a test network like Rinkeby. Install a Solidity compiler, such as Remix.
2. Write and compile your contract: Write your contract code in Solidity, then compile it using the compiler.
3. Deploy your contract: Deploy your compiled contract to the blockchain using a tool like Remix or Truffle.
4. Interact with your contract: Write a client-side application, such as a web page or a command line tool, to interact with your contract. Use a library like web3.js to communicate with the blockchain.
5. Test your contract: Write tests for your contract to ensure that it behaves as expected.
6. Deploy to the main network: Once you have tested your contract, you can deploy it to the Ethereum main network.
7. Monitor your contract: Use tools like Etherscan
