## QuickAlerts Community Examples

### Table of Contents
- [QuickAlerts Community Examples](#quickalerts-community-examples)
  - [Table of Contents](#table-of-contents)
  - [What is QuickAlerts by QuickNode?](#what-is-quickalerts-by-quicknode)
  - [How to Use QuickAlerts](#how-to-use-quickalerts)
  - [Community Examples](#community-examples)
    - [Examples](#examples)
  - [Contribution Guide](#contribution-guide)
  - [Contributors](#contributors)

### What is QuickAlerts by QuickNode?
[QuickAlerts](https://www.quicknode.com/quickalerts?utm_source=github&utm_campaign=quickalerts-examples) is an easy-to-use tool for real-time monitoring of blockchain events. QuickAlerts enables you to leverage real-time blockchain data and advanced alerting to power your apps, make DeFi trading decisions based on the specific data that matters to you, add real-time blockchain event driven logic into your workflows, and more. Monitor over 6 blockchains and 8 networks in real time!

Quickly set up alerts for events that occur on over 6 different blockchains and 8 different networks. You can monitor smart contracts for specific events, such as a contract being deployed, a transaction being sent to a specific address, and much more. When an event occurs, QuickAlerts will notify you in real-time via webhook.

QuickAlerts is easy to use, and it doesn't require any coding knowledge. You can set up alerts using a simple web interface, and you can customize the alerts to fit your specific needs. Whether you're a developer, a trader, or just a blockchain enthusiast, QuickAlerts can help you stay informed and make more informed decisions.

### How to Use QuickAlerts
[![How to get notified of blockchain events in real-time with QuickAlerts](https://user-images.githubusercontent.com/70228897/219116132-a1bc5201-d873-4f0c-a219-f180f117255a.png)](https://www.youtube.com/watch?v=Y3UZDxX-ZD8)
_Follow our step-by-step tutorial on [YouTube](https://www.youtube.com/watch?v=Y3UZDxX-ZD8)_

To use QuickAlerts, you'll need to create an account on the [QuickNode](https://www.quicknode.com/?utm_source=github&utm_campaign=quickalerts-examples) website. Once you have an account, you can create alerts using a predefined expression template or create one on your own.


**To create an alert, follow these steps:**
- Log in to your [QuickNode](https://www.quicknode.com/?utm_source=github&utm_campaign=quickalerts-examples) account and navigate to the QuickAlerts dashboard.
- Click the "Create QuickAlert" button.
- Name your alert and select the chain and network you'd like your alert on.
- Select a Blank Template or one of our pre-defined templates. If you're using an expression from the [example library](#example-library), then click Blank Template.
- Review the expression if you clicked a pre-defined template, or add your expression in the "Create Expression" field.
- Test your expression and hit "Next"
- Create your destination and Deploy your alert!

Once you've created an alert, QuickAlerts will monitor the selected blockchain for the specified event. When the event occurs, QuickAlerts will send you a notification according to the method you chose.

### Community Examples
The examples directory contains a set of example alerts that you can use to get started with QuickAlerts. Each example includes a description of the alert, the conditions for triggering the alert, and the expected result. The examples cover a variety of use cases, such as monitoring token transfers, tracking contract deployments, and detecting large transactions.

To use the example alerts, simply copy the expression details from the example and [follow the How to Use QuickAlerts guide](#how-to-use-quickalerts). 

#### Examples
- ERC721 & ERC1155
  - [Any ERC721 or ERC1155 NFT is Minted](examples/any-nft-is-minted.md)
  - [CryptoPunk Transfered](examples/crypto-punk-transfered.md)
  - [Bored Ape Yacht Club (BAYC) Transfered](examples/bayc-transfered.md)
- ERC20
  - [$BLUR Airdrop Claimed meets a certain threshold of tokens](examples/blur-whale-claims.md)
- Blocks
  - [Block Number Alert - Get alerts when a specific block is mined](examples/block-number-alert.md)
- Transaction
  - [Block Number Alert - Get alerts when a specific block is mined](examples/block-number-alert.md)

### Contribution Guide
We welcome contributions from the community to share their examples! If you'd like to contribute, please follow these guidelines:

- Fork the QuickAlerts repository.
- Create a new branch for your changes.
- Copy the `TEMPLATE.md` file to the `examples` directory and fill out the details.
- Push your changes to your fork.
- Submit a pull request to the main QuickAlerts repository.

We will review your pull request as soon as possible and provide feedback if necessary. Thank you for your contributions!

### Contributors
- [QuickNode](https://www.quicknode.com?utm_source=github&utm_campaign=quickalerts-examples)
