# Smart Contract for CrowdFunding using Solidity :page_facing_up:
#### Second project of IEEE's Workshop: Build your own Blockchain from Cryptocurrency to Smart Contracts

This project implements crowdfunding using smart contracts via solidity in ethereum blockchain technology.

Crowdfunding is a way of funding a project or venture by raising small amounts of money from a large number of people.
A **smart contract** in crowdfunding is a **self-executing agreement** between investors and fundraisers put into the blockchain ecosystem. It acts as a middleman who manages the user's information.

## Smart contract Design:
- The manager of the company sets a **target** of the money to be raised, **deadline** i.e. till when should the target money be raised and **minimum contribution** per investor along with the cause of funding.
- To eliminate the chances of any frauds, the crowd doesn’t pay directly to the manager, instead it gets stored in the form of a smart contract.
- The manager can withdraw the money from the smart contract,only if 50% of the contributors vote to agree to it.
- In case the target and deadline are not fulfilled, the contributors can claim their ethers back.

## How to start executing this smart contract :

1. Upload and Compile the .sol file in Remix IDE. Once it has been compiled and no bugs are detected you can deploy your project.
2. Deploy the project. For this you have to pass in values for 2 fields that is the Target Amount the manager wants to achieve and the Time Duration before which the Target has to be achieved so that accordingly the contract is created.
3. Click on the Deploy button and you are good to go !
4. Here we can select the address of the contributor and accordingly enter the amount of money in the value field along with the units of ether in dropdown. A contributor can send the amount of money he wants to pay using **value** field and **sendETH** function. 
 
<img width="339" alt="crowd2" src="https://user-images.githubusercontent.com/85681285/145810903-5224cb29-5dc5-49df-813c-b6dbd808802f.png">

## Features :
- **sendETH** - A supporter can become a contributor by sending ether by calling this function. Contribution can be made only when the deadline has not passed and a minimum amount of ether has been funded.
- **refund** - A contributor is entitled to request a refund provided the following conditions are met : Deadline has passed and the target has not been reached. Once it is verified that the person is a valpid contributor, smart contract will make the refund.
- **createRequests** - Only the manager can call this function by giving the following parameters (description of the project i.e why companies should invest in the project, account address as to where the collected fund has to be transferred and the target of the particular fund raiser)
- **voteRequest** - A function that will take a vote into consideration if the contributor is valid and has not voted previously.
- **makePayment** - Only the manager can call this function. If the amount raised is equal to or more than the target and the majority is in favor of the manager then he can execute this function and credit the funds that he has raised to the address provided while creating the request.

<img width="321" alt="crowd1" src="https://user-images.githubusercontent.com/85681285/145810698-28d1ff36-1498-4c83-8c07-d5a35d0c518d.png">

#### The first 4 fields in above image represent functions and the remaining fields are the public variables used in this smart contract.

## Conclusion :
- As per the problem statement we have successfully created a smart contract which is built in such a way that it ensures well structured functioning as per our design. 
- With help of such smart contracts proper funding for a particular project or any other purpose can be done as the contract ensures that Contributors are availed to all the facilities mentioned in the policy. 
- Such smart contracts can be used to overcome various problem statements for example, voting system where political leaders can manipulate the results, traditional home agreements which can be easily manipulated by hacking the system or because of political powers, etc
- Hereby we can conclude that deploying smart contracts can prove to be useful in order to overcome various problem statements and mallicious activities with the help of proper knowledge of that particular domain and the technology behind smart contracts.
