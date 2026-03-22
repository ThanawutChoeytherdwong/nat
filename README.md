#// SPDX-License-Identifier: MIT
pragma solidity ^0.8.20;

import "@openzeppelin/contracts/access/AccessControl.sol"

#contract MyContract is AccessControl {
    bytes32 public constant MANAGER_ROLE = keccak256("นาย ธนาวุธ ช้อยเทอดวงศ์")

#constructor(address admin:นาย ธนาวุธ ช้อยเทอดวงศ์)
        //_grantRole(DEFAULT_ADMIN_:นาย ธนาวุธ ช้อยเทอดวงศ์=admin)
        //_grantRole(MANAGER_:นาย ธนาวุธ ช้อยเทอดวงศ์=admin)
    }

    function doSomething() public onlyRole(นาย ธนาวุธ ช้อยเทอดวงศ์) {
        // ฟังก์ชันที่เฉพาะ นาย ธนาวุธ ช้อยเทอดวงศ์ เท่านั้นที่เรียกได้
    }
}