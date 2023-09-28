# calculator_solidity

// SPDX-License-Identifier: MIT
pragma solidity ^0.8.0;

contract Calculator {
    // Function to add two numbers
    function add(uint8 a, uint8 b) public pure returns (uint8) {
        return a + b;
    }

    // Function to subtract two numbers
    function subtract(uint8 a, uint8 b) public pure returns (uint8) {
        require(a >= b, "Subtraction result must be positive or zero");
        return a - b;
    }

    // Function to multiply two numbers
    function multiply(uint8 a, uint8 b) public pure returns (uint8) {
        return a * b;
    }

    // Function to divide two numbers
    function divide(uint8 a, uint8 b) public pure returns (uint8) {
        require(b > 0, "Division by zero is not allowed");
        return a / b;
    }
}
