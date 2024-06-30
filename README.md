# Savings account smart contract using require(),assert(),revert()

## Description

Savings is the name of the Solidity contract that oversees a straightforward bank account that includes deposit and withdrawal capabilities. The account balance is monitored by the public balance, current, which is maintained by the contract. The deposit function allows users to transfer funds, which will increase the balance. However, the transaction will be reversed if the balance exceeds 500,000 units. The withdraw function enables users to withdraw funds by verifying that the balance is sufficient prior to executing the withdrawal. The isempty function determines whether the balance is zero and returns a message if it is. Basic financial operations for a savings account are provided by the contract, which also guarantees balance constraints.

## Getting Started

### Executing program
require(balance > amount, "You do not have enough balance to transfer!");
This line is a condition that checks if the balance is larger than the stated amount. If it's not, the function will reverse the transaction and display the error message "You do not have enough balance to transfer!".

balance -= amount; This line subtracts the amount from the balance.

function deposit(uint amount) public { ... } This line declares a public function named deposit that accepts a parameter amount of type uint and does not return any value.

balance += amount; This statement adds the amount to the balance.
All three commands for solidity used in this project are
code blocks for commands
```
        require(current > money, " Transaction failed due Insuffficient balance for the transfer!");

        revert("You cannot further deposit money as your balance is exceeding the limit!");
        
        assert(current == 0);
```

## Authors

ex. Arpan Kumar  
ex. [ironextreme5@gmail.com]


## License

This project is licensed under the [MIT] License - see the LICENSE.md file for details
