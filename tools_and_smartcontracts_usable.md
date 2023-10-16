1. Problem reentrancy
   https://github.com/topics/reentrancy

   historical attacks

    https://github.com/pcaversaccio/reentrancy-attacks

   solution:
   is https://ethamal.medium.com/a-look-at-open-zeppelins-reentrancyguard-6ff3590d0719

   https://github.com/OpenZeppelin/openzeppelin-contracts/blob/master/contracts/utils/ReentrancyGuard.sol

       /**
     * @dev Prevents a contract from calling itself, directly or indirectly.
     * Calling a `nonReentrant` function from another `nonReentrant`
     * function is not supported. It is possible to prevent this from happening
     * by making the `nonReentrant` function external, and making it call a
     * `private` function that does the actual work.
  
     */

   you must make your smartcontract to inherit from ReentrancyGuard
   so YourSmartContract is ReentrancyGuard 
2. Arithmetic Overflow and Underflow only in version 0.6 and 0.7 
notice that in 0.8 and above this vulnerability is covered. Now it throws error.
3. 
