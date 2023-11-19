# MyToken

## Functionality

1. **Token Initialization**
   - The contract is initialized with an initial supply of tokens, and the owner receives the entire supply.

2. **Mint Tokens**
   - `mint(uint256 amount) public onlyOwner`: Allows the owner to mint additional tokens and add them to the total supply.

3. **Burn Tokens**
   - `burn(uint256 amount) public`: Allows users to burn their own tokens, subject to certain conditions. The amount to burn must be greater than 10, and the user must have a sufficient balance.

4. **Token Transfer**
   - `transfer(address to, uint256 amount) public override returns (bool)`: Overrides the ERC-20 `transfer` function to provide custom logic.
