# shibaswap-contracts 
# Security Policy

## Supported Versions

Use this section to tell people about which versions of your project are

currently being supported with security updates.

| Version | Supported          |

| ------- | ------------------ |

| 5.1.x   | :white_check_mark: |

| 5.0.x   | :x:                |

| 4.0.x   | :white_check_mark: |

| < 4.0   | :x:                |

## Reporting a Vulnerability

Use this section to tell people how to report a vulnerability.

Tell them where to go, how often they can expect to get an update on a

reported vulnerability, what to expect if the vulnerability is accepted or

declined, etc.

# pragma solidity >=0.5.0;

interface IERC20 {

    event Approval(address indexed owner, address indexed spender, uint value);

    event Transfer(address indexed from, address indexed to, uint value);

    function name() external view returns (string memory);

    function symbol() external view returns (string memory);

    function decimals() external view returns (uint8);

    function totalSupply() external view returns (uint);

    function balanceOf(address owner) external view returns (uint);

    function allowance(address owner, address spender) external view returns (uint);

    function approve(address spender, uint value) external returns (bool);

    function transfer(address to, uint value) external returns (bool);

    function transferFrom(address from, address to, uint value) external returns (bool);

}
