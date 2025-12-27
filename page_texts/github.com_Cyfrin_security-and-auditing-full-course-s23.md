# GitHub - Cyfrin/security-and-auditing-full-course-s23: The ultimate, most advanced, security, DeFi, assembly, web3 auditor course ever created.

**URL:** https://github.com/Cyfrin/security-and-auditing-full-course-s23

---

Skip to content
Navigation Menu
Platform
Solutions
Resources
Open Source
Enterprise
Pricing
Sign in
Sign up
Cyfrin
/
security-and-auditing-full-course-s23
Public
Notifications
Fork 417
 Star 1.8k
Code
Issues
3
Pull requests
Discussions
Actions
Security
Insights
Cyfrin/security-and-auditing-full-course-s23
 main
7 Branches
0 Tags
Code
Folders and files
Name	Last commit message	Last commit date

Latest commit
Equious
Merge pull request #412 from odupontt/link2
da8887a
 · 
History
107 Commits


.github
	
Increase quality on the Powered by Cyfrin badge (#21)
	


images
	
Add file top-10-2025 via upload and update Readme
	


.gitignore
	
update
	


.gitmodules
	
Part 2 updated (#146)
	


CODE_OF_CONDUCT.md
	
Fix typos in CODE_OF_CONDUCT.md
	


CONTRIBUTING.md
	
fix-grammar-typos (#368)
	


LICENSE
	
license
	


README.md
	
fix: Update Google Bard link to Gemini
	


TODO.md
	
sepolia challenges
	


chronological-updates.md
	
Fix broken links
	


cookbook-listings.md
	
Update description for cookbook in README.md and cookbook-listings.md (…
	


eip712hashing.sol
	
Fix ecrecover zero-address vulnerability
	


extensive-onboarding-questions.md
	
updated
	


finding_layout.md
	
added finding layout
	


how-to-answer-a-question.md
	
fix-grammar-typos (#368)
	


how-to-ask-a-question.md
	
fix-grammar-typos (#368)
	


improvement_points.md
	
fix-grammar-typos (#368)
	


media-kit.md
	
update
	


minimal-onboarding-questions.md
	
updated
	
Repository files navigation
README
Code of conduct
Contributing
GPL-3.0 license
Smart Contract Auditing, Assembly, Security, and DeFi Ultimate Course

Level up your career as a smart contract auditor writing secure and optimized smart contracts.

    


 


And The Red Guild

Welcome to the repository for the Ultimate Smart Contract Auditing, Assembly, Security, and DeFi Course by Cyfrin Updraft and The Red Guild!

[IMPORTANT!] Course Link: https://updraft.cyfrin.io/courses/security

This repository houses the written content of our courses, organized to facilitate easy access and contribution from our community. Please refer to this for an in-depth explanation of the content:

Website - Join Cyfrin Updraft and enjoy 50+ hours of smart contract development courses
Twitter - Stay updated with the latest course releases
LinkedIn - Add Updraft to your learning experiences
Discord - Join a community of 3000+ developers and auditors
Newsletter - Weekly security research tips and resources to level up your career
Codehawks - Smart contracts auditing competitions to help securing web3






Table of Contents

Note: If you're familiar with Patrick's previous courses, we have renamed "Lessons" to "Sections"

Smart Contract Auditing, Assembly, Security, and DeFi Ultimate Course
Smart Contract Auditing, Assembly, Security, and DeFi Ultimate Course
Table of Contents
Introduction, Resources, and Prerequisites
Curriculum
🤗 Section 0: Welcome to the Course
🐸 Section 1: Review (Don't skip)
❓ Section 2: What is a smart contract audit (Security Review)?
⛳️ Section 3: Your first audit | PasswordStore Audit
🐶 Section 4: Manual & Static Analysis | Puppy Raffle Audit
🔄 Section 5: Invariants & Intro to DeFi | TSwap Audit
🌩️ Section 6: Centralization, Proxies, and Oracles | Thunder Loan Audit
🌉 Section 7: Bridges, Chains, Signatures, Intro to Yul/Assembly | Bridge Boss Audit
🛡️ Section 8: (THE FINAL BOSS AUDIT) MEV, Nodes, & DAOs | Vault Guardians Audit
First CodeHawks Competitive Audit
Congratulations
Thank you
Introduction, Resources, and Prerequisites

Head over to the Cyfrin Updraft website to get the best learning experience!

Link to course: https://updraft.cyfrin.io/courses/security

⚠️ All code associated with this course is for demo purposes only. They have been audited, but we do not recommend them for production use and should be used at your own risk.

Resources For This Course

Join Cyfrin Updraft for the best learning experience!

AI Frens
ChatGPT
Just know that it will often get things wrong, but it's very fast!
Phind
Like ChatGPT, but it searches the web
Gemini
Other AI extensions
devdacian - ai auditor primers - Collection of prompts to improve LLM performance for smart contracts from cyfrin's lead auditor
Github Discussions
Ask questions and chat about the course here!
Stack Exchange Ethereum
Great place for asking technical questions about Ethereum
Peeranha
Decentralized Stack Exchange!
Cookbook
A smart contract registry and co-pilot
Exploit Resources
SC Exploits Minimized
Signature Verification
wise-signer
Challenge Contracts Registry
Challenge Contracts (zkSync)
Challenge Contracts (zkSync Sepolia)
Challenge Contracts (Sepolia)
Prerequisites

An intermediate understanding of solidity. You don't need to be a pro, but you should be familiar with:

Blockchain basics (transactions, blocks, decentralization, etc)
Running a smart contract test suite (hardhat, foundry, truffle, etc)
Solidity basics (variables, functions, structs, etc)

Here are some resources to get you up to speed with the prerequisites:

Full Foundry Course: This will give you every single prerequisite
Speed Run Ethereum: This will give you most of what you need. But you’ll need a little extra time on invariant tests, using foundry, and DeFi/OnChain Finance.
Prerequisite tools
git
foundry
VSCode or other text editor
Understand Markdown syntax
ChatGPT or other AI assistant
Outcome
Have the foundational skills to become a professional smart contract auditor
Speak, interact, and contribute to the web3 security community
Compete in web3 competitive audits
Compete in web3 bug bounties
Start a career as an independent auditor
Become a top 1% smart contract developer
Bonus NFTs
You can find them on zkSync here
It's just numbers 0 -> 8
Important Notes for zkSync

IF YOU DECIDE TO MINT THE REAL NFT:

We didn't audit/security review the NFT, so if you want to make sure you'll be safe, interact with the contract using a burner wallet (a wallet with very little money that you don't use for anything else)
In fact... Get good at interacting with wallets from a burner wallet
Read my Tweet thread on basic wallet safety
Bridging to zkSync
We didn't show you how to bring ETH -> zkSync, but the process would be:
Buy ETH (On an exchange like Coinbase or Kraken)
Send ETH -> one of your wallets like:
Safe (Multi-Sig)
Metamask
Frame
Rainbow
Argent
Coinbase Wallet
Use the zkSync Bridge
Curriculum
🤗 Section 0: Welcome to the Course

Do not skip this section!

Welcome
Why Web3 Security?
Web3 is important
Permissionless finance
Unbreakable promises
Web3 security is subpar right now
Rekt Leaderboard
$1B in 2023 (so far)
Web3 vs Web2 hacks. Web2 is mostly PII theft, where Web3 hacks result in irrevocable losses of funds.
Bad actors in the space. Lone wolf hackers vs. well funded, persistent nation state actors (e.g. NK).
Career opportunities
Top 1% Developer
Private Audits
Cyfrin
Trail Of Bits
Independent Security Researcher
Competitive Audits
CodeHawks
Code4rena
Bug Bounties
$2.2M Payout
Immunefi
Hats Finance
Future:
Incident Responders
On-chain investigators
More…
Why Web3 is so important

Rebuild trust in the ecosystem.

Wild West image to the outsiders

Pick a class

The Final Boss Codebase, you'll be able to audit this at the end of this course
Vault Guardians
Best Practices for this course
Register for Cyfrin Updraft
USE THIS SITE!!! It's specifically made to make learning easier
Follow the repository: While going through the course be 100% certain to follow along with the github repository. If you run into in an issue check the chronological-updates in the repo.
Be Active in the community: Ask questions and engage with other developers going through the course in the discussions tab, be sure to go and say hello or gm! This space is different from the other industries, you don't have to be secretive; communicate, network and learn with others :)
Learn at your own pace: It doesn't matter if it takes you a day, a week, a month or even a year. Progress >>> Perfection
Take Breaks: You will exhaust your mind and recall less if you go all out and watch the entire course in one sitting. Suggested Strategy every 25 minutes take a 5 min break, and every 2 hours take a longer 30 min break
Refer to Documentation: Things are constantly being updated, so whenever Patrick opens up some documentation, open it your end and maybe even have the code sample next to you.
Use ChatGPT and/or the course chat

And finally, by embarking on this journey, you are now a "Security Researcher", not an "Auditor". The key word is "Researcher", so we will go over strategies for continued learning so you can stay on top of your game.

🎯🎯🎯🎯🎯🎯🎯🎯🎯🎯🎯🎯🎯🎯🎯🎯🎯🎯🎯🎯🎯🎯🎯

🎯 Exercise: Write yourself a message about why you want this

This will be important for when things get hard
Is it money? Save web3? Become someone? Write down as many reasons as possible.
Section 0 NFT
Welcome! (zkSync)
Welcome! (Sepolia)

🎯🎯🎯🎯🎯🎯🎯🎯🎯🎯🎯🎯🎯🎯🎯🎯🎯🎯🎯🎯🎯🎯🎯

(back to top) ⬆️

🐸 Section 1: Review (Don't skip)
Tooling & Environment Prerequisites
VSCode
VSCodium
Foundry
chisel
cast
forge
Windows Users: WSL
AI Helpers
ChatGPT
Phind
Forums & Resources
Ethereum Stack Exchange
Peeranha
Github Discussions
Solidity & Smart Contract Prerequisites
Remix
Basic smart contracts
forge init
Fuzzing & Stateful Fuzzing (This might be new)
Fuzz tests
Stateless Fuzzing
Stateful fuzzing
Invariants
Video
Common EIPs/ERCs
Github Copilot
ERC20s
Video
NFTs (ERC721s)
Video
Advanced Solidity
storage
Clip from foundry course
Fallback & Receive
Encoding, Call, & Staticcall
Clip from the foundry full course
Encoding.sol
CallAnything.sol
Delegatecall & Proxies
Clip from foundry full course
tx.origin vs msg.sender
Selfdestruct (to be removed in an upcoming fork)
Solidity by example
Advanced Foundry
mainnet-forking

🐸🐸🐸🐸🐸🐸🐸🐸🐸🐸🐸🐸🐸🐸🐸🐸🐸🐸🐸🐸🐸🐸🐸

🐸 Exercise:

Join the CodeHawks/Cyfrin Discord
Go for a walk, and buckle up
Section 1 NFT
Refresher Fresh NFT (zkSync)
Refresher Fresh NFT (Sepolia)

🐸🐸🐸🐸🐸🐸🐸🐸🐸🐸🐸🐸🐸🐸🐸🐸🐸🐸🐸🐸🐸🐸🐸

(back to top) ⬆️

❓ Section 2: What is a smart contract audit (Security Review)?
What is a security review/smart contract audit?
High Level Overview
People say "audit" -> security review
There is no silver bullet to auditing, and they have limitations
3 phases of a security review
Initial Review
Scoping
Reconnaissance
Vulnerability identification
Reporting
Protocol fixes
Fixes issues
Retests and adds tests
Mitigation Review
Reconnaissance
Vulnerability identification
Reporting
Smart Contract Development Life Cycle
Plan & Design
Develop & Test
Smart Contract Audit & Post Deploy Planning
Is this just one step?
Deploy
Monitor & Maintain
Top Smart Contract Auditors (Subjective!)
Use this list to reference how top quality security teams do reviews, post reports, do research, etc
Audit Readiness
Simple Security Checklist
Test suite with code coverage
Fuzzing, Static Analysis
Natspec (especially for external/public functions)
The Rekt Test
”Code maturity” is important!
Tooling
Static Analysis
Slither
Aderyn
Fuzzing / Invariant Tests
Foundry
Echidna
Consensys
Formal Verification
Certora
Solidity SMT Checker
Maat
Manticore
AI
Tooling vs Humans
Attacker vs. Defender mindset
Always learning
Top Attack Vectors
Top attack vectors






📝📝📝📝📝📝📝📝📝📝📝📝📝📝📝📝📝📝📝📝📝📝📝

📝 Exercise: Sign up for one security/web3 newsletter!

Cyfrin Updraft
Blockchain Threat Intelligence (Referral link)
Solodit (not a newsletter, but has constant updates of new hacks)
rekt
Week In Ethereum (here's why)
Consensys Diligence Newsletter
Officer CIA
Section 2 NFT
Hardest one of the whole course (zkSync)
Hardest one of the whole course (Sepolia)

📝📝📝📝📝📝📝📝📝📝📝📝📝📝📝📝📝📝📝📝📝📝📝

(back to top) ⬆️

🟢🟢🟢🟢🟢🟢🟢🟢🟢🟢🟢🟢🟢🟢🟢🟢🟢🟢🟢🟢🟢🟢🟢

Important Note: We are now going to do audits. Please note, that we will not find all the bugs in each codebase. Each codebase was designed to show you a specific set of bugs, and give you a good understanding of what an audit "feels" like.

🟢🟢🟢🟢🟢🟢🟢🟢🟢🟢🟢🟢🟢🟢🟢🟢🟢🟢🟢🟢🟢🟢🟢

⛳️ Section 3: Your first audit (security review) | PasswordStore Audit






💻 Security Review CodeV1: https://sepolia.etherscan.io/address/0x2ecf6ad327776bf966893c96efb24c9747f6694b

💻 Security Review CodeV2: https://github.com/Cyfrin/3-passwordstore-audit

💻 Security Review CodeV3: https://github.com/Cyfrin/3-passwordstore-audit/tree/onboarded

💻 Security Review Final: https://github.com/Cyfrin/3-passwordstore-audit/tree/audit-data

Feel free to look ahead and try to find the bugs on the codebase yourself, or get familiar with the protocol first.

Remember the phases!

🔽🔽🔽🔽🔽🔽🔽🔽🔽🔽

Initial Review
Scoping
Reconnaissance
Vulnerability identification
Reporting

🔼🔼🔼🔼🔼🔼🔼🔼🔼🔼

For this demo, we are ignoring the last 2 phases

Protocol fixes
Fixes issues
Retests and adds tests
Mitigation Review
Reconnaissance
Vulnerability identification
Reporting
The Setup (Scoping): PasswordStore
V1
"Hey, here is my link to Etherscan, can I get an audit?"
Coinbase asset listing guide
V2
Client onboarding: Minimal
V3
cloc
"The Tincho"
Read docs
Note taking in-code
Small -> Large
Solidity Metrics
Tincho’s ENS Review
Exploits (Vulnerability Identification)
Exploits: Access Controls
Missing onlyowner
Access Controls
Unprotected sensitive functions
Role misconfiguration
Privilege escalation
Exploits: Private Data
Storing a secret (private data is not private)
More Recon
coverage
Writing your first finding
Write finding
How to write a good finding
Title: Root Cause + Impact
Finding Layout:
### [S-#] Title (ROOT CAUSE + IMPACT)

**Description:** 

**Impact:** 

**Proof of Concept:**

**Recommended Mitigation:** 

Write PoC
Mitigation
Using AI
Are we done?
Your first report (Reporting)
Writing the Report
Severity Classification
Severity Guide
Basic Markdown Report
Template
Alternative way to generate a PDF report

🥚🥚🥚🥚🥚🥚🥚🥚🥚🥚🥚🥚🥚🥚🥚🥚🥚🥚🥚🥚🥚🥚🥚

🥚 Exercises:

Sign up for CodeHawks!
Tweet about your first audit!
Section 3 NFT
Storage refresher! (zkSync)
Storage refresher! (Sepolia)

🥚🥚🥚🥚🥚🥚🥚🥚🥚🥚🥚🥚🥚🥚🥚🥚🥚🥚🥚🥚🥚🥚🥚

(back to top) ⬆️

🐶 Section 4: Manual & Static Analysis | Puppy Raffle Audit

✅✅✅✅✅✅✅✅✅✅✅✅✅✅✅✅✅✅✅✅✅✅✅✅✅

This is the BEST security review for new auditors, 100% be sure to pay attention to this section.

✅✅✅✅✅✅✅✅✅✅✅✅✅✅✅✅✅✅✅✅✅✅✅✅✅

This is the go-to best starter audit/security review. There are a lot of bugs in here, some obvious, some not.







💻 Security Review Code: https://github.com/Cyfrin/4-puppy-raffle-audit

Concepts you'll learn: Static analysis, Reentrancy, Weak RNG, Arithmetic issues, How to write a professional looking report.

Tooling: Static Analysis
Web3 bugs machine vs human
Static Analysis
Slither
Aderyn
cloc
Solidity Metrics (audit estimation)
Solidity Visual Developer
Scoping & Reconnaissance: Puppy Raffle
Exploits: DoS (Denial of service)
Fixes:
Remove unnecessary loops
Exploits: Reentrancy
Case Study: DAO Hack
Still plagues us today
Exercises
Search "reentrancy" in Solodit
Prevention:
CEI/CEII ( FREI-PI soon!)
NonReentrant modifiers
Exploits: Weak RNG
Case Study: Meebits
Exercises
Search "RNG" in Solodit
Prevention:
Chainlink VRF
Exploits: Arithmetic issues
Examples:
Under/Overflow
Rounding & Precision
Exercises
Search "overflow" in Solodit
Prevention:
Use newer versions of solidity
Multiply before divide
Exploits: Poor ETH Handling
Case study: Sushiswap Miso
Exercises:
Stuck ETH without a way to withdraw
Mishandling ETH
Search "Stuck ETH" in Solodit
Informational Findings
Strict Solc Versioning
Supply Chain Attacks
Magic Numbers
Gas Audits
Code Maturity
Code coverage
Static Analysis, follow up
What is a Competitive Audit?
CodeHawks Docs
Writing the report: Puppy Raffle
Audit Report Templating
Github Report Templating (Cyfrin)
Github Report Templating (Spearbit)
Github Report Templating (Spearbit Custom)

🧑‍🚀🧑‍🚀🧑‍🚀🧑‍🚀🧑‍🚀🧑‍🚀🧑‍🚀🧑‍🚀🧑‍🚀🧑‍🚀🧑‍🚀🧑‍🚀🧑‍🚀🧑‍🚀🧑‍🚀🧑‍🚀🧑‍🚀🧑‍🚀🧑‍🚀🧑‍🚀🧑‍🚀🧑‍🚀🧑‍🚀

🧑‍🚀 Exercises:

Ethernaut Challenges (1, 9, and 10) 🧑‍🚀
Sign up for Solodit
Post a tweet about how you completed the Puppy Raffle Audit!
Sign up for farcaster
Do a CodeHawks First Flight
Section 4 NFT
A combination hack (zkSync)
A combination hack (Sepolia)

🧑‍🚀🧑‍🚀🧑‍🚀🧑‍🚀🧑‍🚀🧑‍🚀🧑‍🚀🧑‍🚀🧑‍🚀🧑‍🚀🧑‍🚀🧑‍🚀🧑‍🚀🧑‍🚀🧑‍🚀🧑‍🚀🧑‍🚀🧑‍🚀🧑‍🚀🧑‍🚀🧑‍🚀🧑‍🚀🧑‍🚀

(back to top) ⬆️

🔄 Section 5: Invariants & Intro to DeFi | TSwap Audit






💻 Security Review Code: https://github.com/Cyfrin/5-t-swap-audit

Concepts you'll learn: Stateful fuzzing, Fuzzing, Invariants, FREI-PI/CEII, Advanced DeFi, AMMs, Uniswap, Curve.fi, Constant product formula

🛑🛑🛑🛑🛑🛑🛑🛑🛑🛑🛑🛑🛑🛑🛑🛑

STOP!

Don't look at the contracts for this one!

We are going to show you how you can use advanced tools to find even more bugs just by properly understanding invariants and writing more effective test suites.

🛑🛑🛑🛑🛑🛑🛑🛑🛑🛑🛑🛑🛑🛑🛑🛑

The Setup (Scoping): T-Swap
Client onboarding: Extensive
Reconnaissance: T-Swap
Protocol Invariants
FREI-PI/CEI
Intro to DeFi/OnChain Finance
DeFi Llama
AMMs
UniswapV1
Curve
Constant Product Formula
Tooling: T-Swap
Forge Fuzzing, Stateful Fuzzing, Invariants
Echidna
Foundry
Consensys
Mutation Testing Introduction
Differential Testing Introduction
Solodit
Properties
Exploits: Weird ERC20s
Token integration checklist
Weird ERC20 List
Rebase & fee-on-transfer
ERC777 reentrancy callbacks
Exploits: Core Invariant breaking
Case Study:
Uniswap
Euler
Design Patterns: T-Swap
FREI-PI / CEII / Pre & Post Checks

💰💰💰💰💰💰💰💰💰💰💰💰💰💰💰💰💰💰💰💰💰💰💰💰💰💰

💰 Exercises:

Write a fuzz test to find a bug in this challenge
Write a tweet thread about an interesting finding from Solodit
Section 5 NFT
A legit DeFi On-Chain Hack (zkSync)
A legit DeFi On-Chain Hack (Sepolia)

💰💰💰💰💰💰💰💰💰💰💰💰💰💰💰💰💰💰💰💰💰💰💰💰💰💰

🎊🎊🎊🎊🎊🎊🎊🎊🎊🎊🎊🎊🎊🎊🎊🎊🎊🎊🎊🎊🎊🎊🎊🎊🎊🎊

Congratulations!!

If you've made it this far in the course and you understand what's going on, you have the skills to start getting paid as a security researcher, doing competitive audits, bug bounties, or even get hired!

But if you want to become one of the best in the world and really secure web3, keep going...

🎊🎊🎊🎊🎊🎊🎊🎊🎊🎊🎊🎊🎊🎊🎊🎊🎊🎊🎊🎊🎊🎊🎊🎊🎊🎊

(back to top) ⬆️

🌩️ Section 6: Centralization, Proxies, and Oracles | Thunder Loan Audit






💻 Security Review Code: https://github.com/Cyfrin/6-thunder-loan-audit

We are starting to get more advanced with DeFi and smart contract issues. Buckle up, we are getting hotter.

Scoping & Reconnaissance: Thunder Loan
DeFi: Borrowing & Lending
Aave
Compound
Oracles
Chainlink
TWAP
Proxies
UUPS & Transparent
Multi-facet Proxy (Diamond)
Foundry Proxies & Upgrades
What are upgradeable smart contracts?
Centralization
Malicious Scope
Don't "yes-man" every audit
Tooling: Thunder Loan
Upgradehub
__init vs __init_unchained
Exploits: Failure to initialize
Case Study: I accidentally killed it
Exploits: Storage collision
Exploits: Centralization
Silent Upgrades
Case Study: Oasis
Exploits: Missing events
Exploits: Bad Upgrade
Exploits: Oracle & Price Manipulation
Flash Loans
Case Study: Alpha Homora
Case Study: Cream Finance
Design Patterns: Thunder Loan
Pull over push

📦📦📦📦📦📦📦📦📦📦📦📦📦📦📦📦📦📦📦📦📦📦📦📦📦📦

📦 Exercises:

YAcademy Proxy
Tweet about how YOU feel about upgradeable smart contracts
Section 6 NFT
It's a bit scary how powerful you've become (zkSync)
It's a bit scary how powerful you've become (Sepolia)

📦📦📦📦📦📦📦📦📦📦📦📦📦📦📦📦📦📦📦📦📦📦📦📦📦📦

(back to top) ⬆️

🌉 Section 7: Bridges, Chains, Signatures, Intro to Yul/Assembly | Bridge Boss Audit






💻 Security Review Code: https://github.com/Cyfrin/7-boss-bridge-audit

Tooling: Boss Bridge
AI
Tenderly
evm diff
We will learn "the Hans'"
Checklist
Scoping & Reconnaissance: Boss Bridge
Precompiles
Case Study: Polygon
Public private key demo
Encoding & Decoding Refresher
Exploits: Opcode Support
Case study: zkSync
Exploits: Signature Replay
Exploits: ERC20 Contract Approval
Exploits: Unlimited Minting
Bridge Hacks
Bridge hacks: Ronin, Poly network, Nomad, Wormhole
Writing the report: Boss Bridge
Design Patterns: Boss Bridge
Emergency stop

💰💰💰💰💰💰💰💰💰💰💰💰💰💰💰💰💰💰💰💰💰💰💰💰💰💰

💰 Exercises:

Damn Vulnerable DeFi Challenges 1, 2, 4
Write a tweet thread about an interesting finding from Solodit
Tweet about how you finished the hardest audit yet!
Read about more historic attacks:
Signature Replay
Merkle tree signature issues
Polygon Double Spend
Nomad Bridge Hack
Section 7 NFT
Tell Vitalik Hi (zkSync)
Tell Vitalik Hi (Sepolia)

💰💰💰💰💰💰💰💰💰💰💰💰💰💰💰💰💰💰💰💰💰💰💰💰💰💰

(back to top) ⬆️

Section 7.5: MEV & Governance





Introduction to MEV
MEV Explained
MEV Explained continued
Toxic MEV
Frontrunning
Sandwich Attacks
non-toxic
Backrunning
MEV Protection
Design
Flashbots Protect
MEVBlocker
Securerpc
MEV in our past security reviews:
Puppy:
Someone can front-run selectWinner to call a refund
T-Swap:
Deadline protection means people can "sandwich" attack you
Thunder Loan:
Users can front run flash loans to make the fees higher or lower
Boss Bridge:
A signed transaction could be front run so that an attacker sends tokens from an L2 before the signer can
Slippage Protection
Exploits: Governance Attack
Unlimited Minting
Flash Loan Voting
Case Study: Beanstalk
Metamorphic upgrades
Case Study: TORN Governance
🛡️ Section 8: (THE FINAL BOSS AUDIT) MEV, Nodes, & DAOs | Vault Guardians Audit






This security review is optional. It's a LOT of code! But if you choose to do it, you'll get a better idea of what a larger codebase feels like. Being comfortable coming up to a codebase and saying "I'll eventually understand this codebase, but right now I don't" is important!

💻 Security Review Code: https://github.com/Cyfrin/8-vault-guardians-audit

Concepts: Vault Guardians
Tokenized Vaults (ERC-4626)
Yearn Finance
Permit2
Good luck :)

🦅🦅🦅🦅🦅🦅🦅🦅🦅🦅🦅🦅🦅🦅🦅🦅🦅🦅🦅🦅🦅🦅🦅🦅🦅🦅

🦅 Exercises:

1st CodeHawks Competitive Audit
Write a tweet thread about an interesting finding from Solodit
Write a blog or tweet on your experience!
Read these tips for auditing multi-chain protocols
Section 8 NFT
GO OUT THERE AND GET IT!!! (zkSync)
GO OUT THERE AND GET IT!!! (Sepolia)

🦅🦅🦅🦅🦅🦅🦅🦅🦅🦅🦅🦅🦅🦅🦅🦅🦅🦅🦅🦅🦅🦅🦅🦅🦅🦅

🦅🦅🦅🦅🦅🦅🦅🦅🦅🦅🦅🦅🦅🦅🦅🦅🦅🦅🦅🦅🦅🦅🦅🦅🦅🦅

First CodeHawks Competitive Audit
How to submit a finding
How to decide severity
Where to find a competitive audit

🦅🦅🦅🦅🦅🦅🦅🦅🦅🦅🦅🦅🦅🦅🦅🦅🦅🦅🦅🦅🦅🦅🦅🦅🦅🦅

🦅🦅🦅🦅🦅🦅🦅🦅🦅🦅🦅🦅🦅🦅🦅🦅🦅🦅🦅🦅🦅🦅🦅🦅🦅🦅

(back to top) ⬆️

🎊🎊🎊🎊🎊🎊🎊🎊🎊🎊🎊🎊🎊🎊🎊🎊🎊🎊🎊🎊🎊🎊🎊🎊🎊🎊

Congratulations!!

If you've made it this far in the course and you understand what's going on, you have the skills to become one of the top security researchers in web3! Either as a solo auditor, freelancer, competitive auditor, or even get hired by a top firm!

However... if you want to be on the cutting edge and be able to understand every nook in web3, you've got a little more to go...

🎊🎊🎊🎊🎊🎊🎊🎊🎊🎊🎊🎊🎊🎊🎊🎊🎊🎊🎊🎊🎊🎊🎊🎊🎊🎊

Part 2 has been moved!
Update on Wallets, Post-deployment, EVM Opcodes, Assembly, and Formal Verification

The next sections (originally just called "part 2") have been moved to their own courses!

Wallets & Post Deployment
Updraft
GitHub
Assembly, EVM Opcodes, and Formal Verification
Updraft
GitHub
Highly Recommend

We highly recommend taking these two courses (linked above) so you can have a thorough grasp of all things EVM.

(back to top) ⬆️

Congratulations

🎊🎊🎊🎊🎊🎊🎊🎊🎊🎊🎊🎊 Completed The Course! 🎊🎊🎊🎊🎊🎊🎊🎊🎊🎊🎊🎊

If you've made it this far... wow.

Where do I go now?
Competitive Audits
CodeHawks
We are working on many things to get you more deals. Stay tuned...
Code4rena
Hats Finance
CodeHawks Discord
Start marketing your services
Twitter, Farcaster, LinkedIn, etc
Blogging: Medium, Mirror, etc
Bug Bounties
Immunefi
Hats Finance
Learning More
Patrick Collins YouTube
Solodit
Block Threat Intelligence (Referral Link)
Consensys Diligence Newsletter
Owen Thurm YouTube
JohnnyTime
The Red Guild YouTube
Cyfrin YouTube
Disclosures

The Cyfrin team runs CodeHawks, Cyfrin Updraft, and private security reviews. They are an advisor to the Peeranha project, and run various blockchain nodes like Chainlink & Ethereum. Additionally, they are responsible for the creation of the Aderyn and Solodit tools.

Thank you
Sponsors
Cyfrin
Updraft
CodeHawks
Solodit
The Red Guild
Lead Lecturers / Code Builders
Patrick Collins | Cyfrin
Tincho | The Red Guild
Guest Lecturers
Josselin Feist | Trail of Bits
Trail of Bits
Fuzzing & Formal Verification
Owen | Guardian Audits
Guardian Audits
Denial Of Service
Andy Li | Sigma Prime
Sigma Prime
Weak Randomness
JohnnyTime | Gingersec
Gingersec
Governance Attack (Specific)
Pashov | Independent Security Researcher
MEV
Juliette | Cyfrin
Governance Attack (General)
Alex Roan | Cyfrin
Fuzzing & Smart Engineering
Special thanks
hansfriese
carlitox477
0Kage
giovannidisiena.eth
Dacian
Alex Roan
Peter Kacherginsky
Karma Coma
Zach Obront
Pinata (for hosting my cringe)
More Security Stuff
Self accounts "audit"
https://scsfg.io/
https://github.com/OffcierCia/Crypto-OpSec-SelfGuard-RoadMap
https://github.com/transmissions11/solcurity
https://github.com/OpenCoreCH/smart-contract-auditing-heuristics
https://secure-contracts.com/
https://github.com/crytic/properties
Sponsors

Big thanks to our sponsors/donors!!

Matter Labs (zkSync)
Arbitrum Foundation
Chainlink Labs
Huge Extra Thank YOU

Thanks to everyone who is taking, participating in, and working on this course. These courses are passion project data dumps for everyone in the web3 ecosystem.

Let's level up so we can keep web3 safer, and thank you again for taking this course!

 

(back to top) ⬆️

About

The ultimate, most advanced, security, DeFi, assembly, web3 auditor course ever created.

Topics
security ethereum cryptocurrency solidity smart-contract-audit
Resources
 Readme
License
 GPL-3.0 license
Code of conduct
 Code of conduct
Contributing
 Contributing
 Activity
 Custom properties
Stars
 1.8k stars
Watchers
 31 watching
Forks
 417 forks
Report repository


Releases
No releases published


Packages
No packages published



Contributors
22
+ 8 contributors


Languages
Solidity
100.0%
Footer
© 2025 GitHub, Inc.
Footer navigation
Terms
Privacy
Security
Status
Community
Docs
Contact
Manage cookies
Do not share my personal information