# errorHandling
In this file we are handling the error using require(), revert() and assert() function.
```
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.18;
contract Error {
    function testRequire(uint _i) public pure {
        require(_i>10, "Input must be greater than 10");
    }
    function testRevert(uint _i) public pure {
        if(_i<=10) {
            revert("Input must be greater than 10");
        }
    }
    uint public num;
    function testAssert() public view {
        assert(num==0);
    }
}
```




