# ErrorHandling Contract

This is a Solidity smart contract that demonstrates different error handling techniques using `assert`, `revert`, and `require` functions.

## License

This contract is using the MIT License.

## Prerequisites

- Solidity ^0.8.17

## Contract Details

The `ErrorHandling` contract provides the following functions:

### Assert(uint num)`

- This function demonstrates the usage of the `assert` function.
- It takes a `num` parameter and checks if it is not equal to zero using the `assert` statement.
- If the condition fails, it triggers an "Internal error" and aborts the execution.

### `multiply(uint _first, uint _second)`

- This function demonstrates the usage of the `revert` function.
- It takes `_first` and `_second` as parameters and performs multiplication.
- It checks if the _first and _second parameters are 0 or not, if they're 0 it will revert the tx 
- If the condition is met, it returns the result of the multiplication

### `divide(uint num2)`

- This function demonstrates the usage of the `require` function.
- It takes a `num2` parameter and performs division with a predefined constant `b`.
- It first checks if `num2` is greater than zero using the `require` statement.
- If the condition fails, it reverts the transaction with a custom error message stating that the value of `num2` should not be zero as denominator should not be 0.
- If the condition is met, it returns the result of the division.

## Usage

1. Make sure you have Solidity ^0.8.17 installed.
2. Compile and deploy the `ErrorHandling` contract to a supported Ethereum network.
3. Interact with the deployed contract by calling the available functions and providing the required parameters.
