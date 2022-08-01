1. [UniswapV2Factory](https://cn.etherscan.com/address/0x5c69bee701ef814a2b6a3edd4b1652cb9cc5aa6f)

   Line 401, add

   ```
   bytes32 public constant INIT_CODE_PAIR_HASH = 
       keccak256(abi.encodePacked(type(UniswapV2Pair).creationCode));
   ```

   


2. [WETH9](https://cn.etherscan.com/address/0xc02aaa39b223fe8d0a0e5c4f27ead9083c756cc2)

3. [UniswapV2Router02](https://cn.etherscan.com/address/0x7a250d5630b4cf539739df2c5dacb4c659f2488d)

   Line 700, modify, from contract1-UniswapV2Factory

   ```
   hex'96e8ac4277198ff8b6f785478aa9a39f403cb768dd02cbee326c3e7da348845f' // init code hash
   ```

4. [Multicall](https://cn.etherscan.com/address/0x5e227ad1969ea493b43f840cff78d08a6fc17796)