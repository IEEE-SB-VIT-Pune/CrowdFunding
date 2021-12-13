# Smart Contract for CrowdFunding using Solidity
##### Second project of IEEE's Workshop: Build your own Blockchain from Cryptocurrency to Smart Contracts

This project implements crowdfunding using smart contracts via solidity in ethereum blockchain technology.

Crowdfunding is a way of funding a project or venture by raising small amounts of money from a large number of people.
A **smart contract** in crowdfunding is a **self-executing agreement** between investors and fundraisers put into the blockchain ecosystem. It acts as a middleman who manages the user's information.

### Smart contract Design:
- The manager of the company sets a **target** of the money to be raised, **deadline** i.e. till when should the target money be raised and **minimum contribution** per investor along with the cause of funding.
- To eliminate the chances of any frauds, the crowd doesn’t pay directly to the manager, instead it gets stored in the form of a smart contract.
- The manager can withdraw the money from the smart contract,only if 50% of the contributors vote to agree to it.
- In case the target and deadline are not fulfilled, the contributors can claim their ethers back.



## Features- 
- **sendETH** - A supporter can become a contributor by sending ether by calling this function. Contribution can be made only when the deadline has not passed and a minimum amount of ether has been funded.
- **refund** - A contributor is entitled to request a refund provided the following conditions are met : Deadline has passed and the target has not been reached. Once it is verified that the person is a valid contributor, smart contract will make the refund.
- **createRequests** - Only the manager can call this function by giving the following parameters (description of the project i.e why companies should invest in the project, account address as to where the collected fund has to be transferred and the target of the particular fund raiser)
- **voteRequest** - A function that will take a vote into consideration if the contributor is valid and has not voted previously.
- **makePayment** - Only the manager can call this function. If the amount raised is equal to or more than the target and the majority is in favor of the manager then he can execute this function and credit the funds that he has raised to the address provided while creating the request.





The first 4 fields represent functions and the remaining fields are the public variables used in this smart contract.







How to start executing this smart contract -
**Step 1:** Compile the .sol file. Once it has been compiled and no bugs are detected you can deploy your project.
**Step 2 :** Deploy the project. For this you have to pass in values for 2 fields that is the Target Amount the manager wants to achieve and the Time Duration before which the Target has to be achieved.
**Step 3 :** Click on the Deploy button and you are good to go !