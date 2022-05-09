# Solidity Joint Account

## Summary of Project

The goal of this project is to automate the creation of joint savings accounts by creating a Solidity smart contract that accepts two user addresses. These addresses will be able to control a joint savings account. The smart contract will use ether management functions to implement a financial institution’s requirements for providing the features of the joint savings account. These features will consist of the ability to deposit and withdraw funds from the account.

## Create a Joint Savings Account Contract in Solidity

The joint_savings.sol file is used in the Remix IDE to implement this project. First, compile the contract. It will look like this when it's compiled and ready to be deployed:

![1](https://raw.githubusercontent.com/tycastleberry/Challenge20/main/Execution_Results/1.png)

 After compiling and deploying the contract, you'll then be able to interact with the contract and test its functionality. It will look like the following at this stage:
 
![2](https://raw.githubusercontent.com/tycastleberry/Challenge20/main/Execution_Results/2.png)
 
 To begin, use the setAccounts function to define the authorized Ethereum address that will be able to withdraw funds from the contract as shown below:

![3](https://raw.githubusercontent.com/tycastleberry/Challenge20/main/Execution_Results/3.png)

Next, deposit 1 ether in wei to the account. Use the contractBalance function to verify the funds were added to the contract.

![6](https://raw.githubusercontent.com/tycastleberry/Challenge20/main/Execution_Results/6.png)

Now deposit 10 either in wei and verify the funds were added again.

![4](https://raw.githubusercontent.com/tycastleberry/Challenge20/main/Execution_Results/4.png)

For the third transaction, send 5 either in wei and verify the funds.

![5](https://raw.githubusercontent.com/tycastleberry/Challenge20/main/Execution_Results/5.png)

Now test the withdrawal functionality by withdrawing 5 ether into accountOne and 10 ether into accountTwo. Verify the funds were withdrawn after each transaction. After withdrawing 5 ether:

![4](https://raw.githubusercontent.com/tycastleberry/Challenge20/main/Execution_Results/4.png)

After withdrawing 10 ether:

![7](https://raw.githubusercontent.com/tycastleberry/Challenge20/main/Execution_Results/7.png)

The final step is to use the lastToWithdraw and lastWithdrawAmount functions to verify that the address and the amount are correct:

![9](https://raw.githubusercontent.com/tycastleberry/Challenge20/main/Execution_Results/9.png)

## Contributors

Tyler Castleberry was the sole contributor to this project. 

---

## License

MIT License

Copyright (c) 2022 Tyler Castleberry

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
