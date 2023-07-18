# ErrorHandling Contract

This is a simple Solidity smart contract named ErrorHandlingExample, which demonstrates different error handling methods using require, assert, and revert. The contract allows setting and retrieving the value state variable while enforcing specific conditions to handle errors gracefully.

## License

This contract is using the MIT License.

## Prerequisites

- Solidity ^0.8.17

## Contract Details

The `ErrorHandling` contract provides the following functions:

### setValueWithRequire

This function sets the value state variable while ensuring that the new_value provided is greater than 0. If the condition fails, the function will revert the transaction with the custom error message "Value must greater than 0".

### getValueWithAssert

This function retrieves the current value stored in the contract's value state variable. Before returning the value, it uses assert to check that the value is not equal to zero. If the condition fails, the function will revert the transaction, indicating an internal error. 

### setValueWithRevert

This function sets the value state variable while ensuring that the new_value2 provided does not exceed 39. If the condition is not met, the function will revert the transaction with the custom error message "Value cannot exceed 39".

## Events

The contract emits two events:

1) ValueSet: This event is emitted whenever the value state variable is successfully set. It includes the newValue as a parameter to indicate the new value assigned to value.

2) ValueGot: This event is emitted when the getValueWithAssert function is called successfully and returns the current value.

## Video Walkthrough

-https://www.loom.com/share/eb656c400a7042c8980bb99c755b5140?sid=9112147f-8b95-4b65-95d8-25589d096e40



