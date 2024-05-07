// SPDX-License-Identifier: MIT
pragma solidity ^0.8.0;

contract ErrorHandlingExample {
    uint public count;

    function increment(uint _value) public {
        require(_value > 0, "Value must be greater than zero"); // Require condition to be true, otherwise revert
        count += _value;
    }

    function decrement(uint _value) public {
        if (_value > count) {
            revert("Value must be less than or equal to count"); // Revert with a message
        }
        count -= _value;
    }

    function assertExample(uint _a, uint _b) public pure returns (uint) {
        uint result = _a + _b;
        assert(result >= _a); // Assert condition to be true, otherwise revert
        return result;
    }
}
