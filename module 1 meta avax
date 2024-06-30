// SPDX-License-Identifier: MIT
pragma solidity ^0.8.0;

contract Savings
{
    
    uint public current = 0;
    function withdraw(uint money ) public   {
        require(current > money, " Transaction failed due Insuffficient balance for the transfer!");
        current -= money;
    }

    function deposit(uint money) public   {
        current += money;
        if (current > 500000) {
            revert("You cannot further deposit money as your balance is exceeding the limit!");
        }
    }
    function isempty() public view returns (string memory){
        assert(current == 0);
        return "Bank balance is NIL.";
    }

}
