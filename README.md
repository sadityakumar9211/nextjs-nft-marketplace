<!-- Improved compatibility of back to top link: See: https://github.com/othneildrew/Best-README-Template/pull/73 -->
<a name="readme-top"></a>
<!--
*** This README is created using template from https://github.com/othneildrew/Best-README-Template
-->



<!-- PROJECT SHIELDS -->
<!--
*** I'm using markdown "reference style" links for readability.
*** Reference links are enclosed in brackets [ ] instead of parentheses ( ).
*** See the bottom of this document for the declaration of the reference variables
*** for contributors-url, forks-url, etc. This is an optional, concise syntax you may use.
*** https://www.markdownguide.org/basic-syntax/#reference-style-links
-->
[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![MIT License][license-shield]][license-url]
[![LinkedIn][linkedin-shield]][linkedin-url]



<!-- PROJECT LOGO -->
<br />
<div align="center">
  <a href="https://github.com/sadityakumar9211/nextjs-nft-marketplace">
    <img width="51" alt="image" src="https://user-images.githubusercontent.com/78147198/187684294-f51b7ada-8fc1-4701-9e5e-3a3fed49c08c.png">
  </a>

  <h2 align="center">NFT Marketplace</h2>
  <h4>Buy NFTs · Sell NFTs · Withdraw Proceeds</h4>
  <p align="center">
    This repository is one of the three repositories which are part of NFT Marketplace Project.
    <br />
    <br>
    <a href="https://github.com/sadityakumar9211/hardhat-nft-marketplace"><strong> <i>hardhat-nft-marketplace</i>: Hardhat Repository of NFT Marketplace Project»</strong></a>
    <br>
    <a href="https://github.com/sadityakumar9211/thegraph-nft-marketplace"><strong> <i>thegraph-nft-marketplace</i>: The Graph Repository of NFT Marketplace Project»</strong></a>
    <br>
    <br />
    <br />
    <a href="https://nftmarketplace-thegraph.vercel.app/">View Demo</a>
    ·
    <a href="https://github.com/sadityakumar9211/nextjs-nft-marketplace/issues">Report Bug</a>
    ·
    <a href="https://github.com/sadityakumar9211/nextjs-nft-marketplace/issues">Request Feature</a>
  </p>
</div>

### This is the Front-end repository of this project. 

<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#requirements">Requirements</a></li>
        <li><a href="#quickstart">Quickstart</a></li>
      </ul>
    </li>
    <li><a href="#locally-deploying">Locally Deploying</a></li>
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#license">License</a></li>
    <li><a href="#contact">Contact</a></li>
    <li><a href="#acknowledgments">Acknowledgments</a></li>
  </ol>
</details>



<!-- ABOUT THE PROJECT -->
## About The Project

<img width="1237" alt="image" src="https://user-images.githubusercontent.com/78147198/187685049-34863fa3-6ea8-46d5-a4d1-85284b4e22c1.png">

**Blockchain** developed the idea of NFTs and introduced digital ownership of certain assets. This is because tokens are not exchangeable which makes it possible to establish property ownership in digital art. 

NFT marketplace is a digital platform to create and trade digital assets. There are several marketplaces to create, sell, buy and trade NFTs. This is one small implementation of such platforms. The platform can allow you to buy and sell NFTs. You can also withdraw funds which you earned after selling the NFTs. For supporting fast and complex queries this system uses a decentralized indexing protocol *The Graph*. The smart contract is currently deployed on *Rinkeby Testnet*.


### The links to other repositories of this project is at the top.
<p align="right">(<a href="#readme-top">back to top</a>)</p>


### Built With

The following is a list of major frameworks, library and tools used for developing this repository.

- [![Next][Next.js]][Next-url]
- [![React][React.js]][React-url]
- [![tailwindcss][tailwindcss]][tailwind-url]
- [![moralis][moralis]][moralis-url]
- [![web3uikit][web3uikit]][web3uikit-url]
- [![pinata][pinata]][pinata-url]


<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- GETTING STARTED -->
# Getting Started

## Requirements

- [git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)
  - You'll know you did it right if you can run `git --version` and you see a response like `git version x.x.x`
- [Nodejs](https://nodejs.org/en/)
  - You'll know you've installed nodejs right if you can run:
    - `node --version` and get an ouput like: `vx.x.x`
- [Yarn](https://classic.yarnpkg.com/lang/en/docs/install/) instead of `npm`
  - You'll know you've installed yarn right if you can run:
    - `yarn --version` and get an output like: `x.x.x`
    - You might need to install it with `npm`
- Optional Instruction
  - Make sure that this repository and `nextjs-nft-marketplace` repository are in the same level in your directory structure.
  - This makes sure that whenever you deploy the smart contract, this repository's `constants` files are updated.
## Quickstart

```bash
git clone https://github.com/sadityakumar9211/nextjs-nft-marketplace
cd nextjs-nft-marketplace
yarn
```

**Note:** If you locally want to run this repository, you have to follow the **Quickstart** and **Deployment** sections of all three repositories of this project. Also make sure that all three repositories are in the same directory when you clone them.   \\

### Optional Gitpod

If you can't or don't want to run and install locally, you can work with this repo in Gitpod. If you do this, you can skip the `clone this repo` part.

[![Open in Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/#github.com/sadityakumar9211/nextjs-nft-marketplace)


<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- USAGE EXAMPLES -->

## Locally Deploying

2. Deploy to your contract to Rinkeby
After installing dependencies, deploy your contracts to rinkeby:

```bash
yarn hardhat deploy --network rinkeby
```


3. Connecting with Subgraph

You can use the same subgraph temporary URI (as present in the `pages/_app.js`) to query the data or you can clone [this repository](https://github.com/sadityakumar9211/thegraph-nft-marketplace) and deploy your own subgraph using the instructions in above repo and generate your own temporary query URI.


4. Start your UI
Make sure that:

In your networkMapping.json you have an entry for `NftMarketplace` on the rinkeby network.
```bash
yarn dev
```
<p align="right">(<a href="#readme-top">back to top</a>)</p>


<!-- CONTRIBUTING -->
## Contributing

Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".
Don't forget to give the project a star! Thanks again!

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- LICENSE -->
## License

Distributed under the MIT License. See `LICENSE` for more information.

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- CONTACT -->
## Contact

If you appreciated this, feel free to follow me or donate!

ETH Address: 0xED5A704De64Ff9699dB62d09248C8d179bb77D8A

[![Aditya Singh Linkedin](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/saditya9211/)
[![Aditya Singh Twitter](https://img.shields.io/badge/Twitter-1DA1F2?style=for-the-badge&logo=twitter&logoColor=white)](https://twitter.com/sadityakumar921)
[![Aditya Singh StackOverflow](https://img.shields.io/badge/StackOverflow-gray?style=for-the-badge&logo=stackoverflow&logoColor=orange)](https://stackoverflow.com/users/14769639/saditya)
[![Aditya Singh Medium](https://img.shields.io/badge/Medium-000000?style=for-the-badge&logo=medium&logoColor=white)](https://medium.com/@sadityakumar9211)
[![Aditya Singh Gmail](https://img.shields.io/badge/Gmail-gray?style=for-the-badge&logo=gmail)](mailto:sadityakumar9211@gmail.com)

Project Link: [https://github.com/sadityakumar9211/nextjs-nft-marketplace](https://github.com/sadityakumar9211/nextjs-nft-marketplace)

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- ACKNOWLEDGMENTS -->
## Acknowledgments

* [Choose an Open Source License](https://choosealicense.com)
* [@apollo/client for querying subgraph](https://www.npmjs.com/package/@apollo/client)
* [daisyui plugin for tailwindcss](https://daisyui.com/)
* [pinata](https://www.pinata.cloud/)


<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/sadityakumar9211/nextjs-nft-marketplace.svg?style=for-the-badge
[contributors-url]: https://github.com/sadityakumar9211/nextjs-nft-marketplace/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/sadityakumar9211/nextjs-nft-marketplace.svg?style=for-the-badge
[forks-url]: https://github.com/sadityakumar9211/nextjs-nft-marketplace/network/members
[stars-shield]: https://img.shields.io/github/stars/sadityakumar9211/nextjs-nft-marketplace.svg?style=for-the-badge
[stars-url]: https://github.com/sadityakumar9211/nextjs-nft-marketplace/stargazers
[issues-shield]: https://img.shields.io/github/issues/sadityakumar9211/nextjs-nft-marketplace.svg?style=for-the-badge
[issues-url]: https://github.com/sadityakumar9211/nextjs-nft-marketplace/issues
[license-shield]: https://img.shields.io/github/license/sadityakumar9211/nextjs-nft-marketplace.svg?style=for-the-badge
[license-url]: https://github.com/sadityakumar9211/nextjs-nft-marketplace/blob/master/LICENSE
[linkedin-shield]: https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white
[linkedin-url]: https://linkedin.com/in/saditya9211
[product-screenshot]: https://user-images.githubusercontent.com/78147198/184471278-42e393d0-db94-4577-bdc9-328510b777c0.png

<!-- This is the beginning of the URLs of Badges -->

[Next.js]: https://img.shields.io/badge/next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white
[Next-url]: https://nextjs.org/
[React.js]: https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB
[React-url]: https://reactjs.org/
[tailwindcss]: https://img.shields.io/badge/tailwindcss-62B9F3?style=for-the-badge
[tailwind-url]: https://tailwindcss.com
[moralis]: https://img.shields.io/badge/moralis-7D9DF0?style=for-the-badge&logoColor=6DE9DB
[moralis-url]: https://moralis.io
[web3uikit]: https://img.shields.io/badge/web3uikit-72E6E0?style=for-the-badge&logoColor=6DE9DB
[web3uikit-url]: https://web3ui.github.io/web3uikit/
[pinata]: https://img.shields.io/badge/pinata-A93FB5?style=for-the-badge&logoColor=6DE9DB
[pinata-url]: https://pinata.cloud/
    

### Deployed to the following URIs:
- IPFS Hash: QmTahM2DWmLq67go9HqPXKSSUdgFTbvqUhErnVeC8r6o9s
- [https://nft-marketplace-saditya9211.on.fleek.co/](https://nft-marketplace-saditya9211.on.fleek.co/)
- [nft-marketpalce-thegraph-sadityakumar9211.vercel.app](https://nft-marketpalce-thegraph-sadityakumar9211.vercel.app)  
- [nft-marketpalce-thegraph-git-main-sadityakumar9211.vercel.app](https://nft-marketpalce-thegraph-git-main-sadityakumar9211.vercel.app)    
- [nft-marketpalce-thegraph.vercel.app](https://nft-marketpalce-thegraph.vercel.app)  













