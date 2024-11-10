# Verifereum 
### First name*

> Ramana

### Last name*

> Kumar

*This should be the main contact we'll be talking to.*

### Email*

> ramana@member.fsf.org


### Organization name*

*Name of your team or organization. If you do not have an organization name, write "N/A".*

> Verifereum

### Team profile*

*Briefly describe your organization. Provide links to previous work. How is your organization suited to the project's objectives, and how does it provide the necessary expertise?*

> Verifereum is currently led by Ramana Kumar. Ramana has a PhD in computer science and has done extensive academic research on formal verification (https://scholar.google.com/citations?user=OyX1-qYAAAAJ&hl=en&oi=sra). They are a world leading expert on compiler verification and a key contributor to CakeML, a verified implementation of ML and one of a handful of formally verified compilers. An active contributor to the liquid staking derivative ecosystem on Ethereum, Ramana combines their expertise in formal verification with a deep knowledge of the EVM. His background makes him uniquely qualified to build Verifereum, an EVM formal verification framework, and Verifereum-based compiler verification projects.
> As the first project to be built on top of Verifereum will be a formally verified version of the Vyper compiler, Ramana will be collaborating closely with cyberthirst (https://github.com/cyberthirst), Vyper's lead security engineer, who is currently working on a definitional interpreter (https://github.com/cyberthirst/ivy/tree/main) in Python. 
> Verifereum also has potential technical (from the CakeML community and academia) and non-technical contributors, although their help will not be necessary for the scope of this grant.
> 

### Twitter

*@Twitter handle for your team or project.*

> N/A

### Website

> https://verifereum.org/

### Project name*

*This should be a concise description of the title of your project.*

> Verifereum

### Project repo

*GitHub or other public repository of the project or related work.*

> [https://github.com/verifereum](https://github.com/verifereum)


### Project category*

*Please choose a category that your project best fits in.*

> Formal Verification

### Brief project summary*

*Describe your project in a few sentences (you'll have the chance to go into more detail in the long form). If it's already underway, provide links to any existing published work.*

> Verifereum is a formal model of Ethereum implemented in higher-order logic (HOL4). For the scope of this grant, we plan to establish a formal specification for a subset of the Vyper programming language (https://github.com/vyperlang/vyper). Specifically a definitional interpreter defined in logic that excludes EVM state operations. We chose Vyper language as its clean design and semantics make it a prime candidate for formal modeling and we plan to eventually expand our work to the whole language and the compiler. 
> In the long term, the project aims to enable the verification of applications and tools within the Ethereum ecosystem, from smart contracts to compilers. Verifereum would not target any specific set of smart contracts or programming languages but is meant to be a general framework for formal verification in the Ethereum space. 


### Describe the current status of the project and progress achieved so far*

*For example, do you have an MVP? Please describe its functionality and limitations and provide a link to it here.*

> Verifereum already has a basic formal model of the EVM in HOL4, available at https://github.com/verifereum/verifereum. While not fully complete, the model is executable and currently passes some tests from the Ethereum Test Set (https://github.com/ethereum/tests). All opcodes are currently implemented and we have started working on implementing the precompiles. Work towards a definitional interpreter targeting the Vyper compiler has also started by formalizing the language's Abstract Syntax Tree (AST) at https://github.com/xrchz/vyper-hol/tree/main. The current formalization is still at an early stage but covers basic types, expressions, and control flow constructs.


### What problem(s) are being solved by within the scope of the grant?*

*What is the specific problems, research questions, or needs you are trying to address?*

> - **Smart contract security:** Over 8 billion dollars have been lost in various hacks (https://defillama.com/hacks) since the launch of Ethereum. By enabling mathematical proofs of contract behavior, Verifereum offers a higher level of security against exploits.
> 
> - **Compiler reliability:** There are currently no formally verified compilers for EVM smart contract programming languages, meaning that there is no fully reliable guarantee that the compiled bytecode will behave as expected from the contract's source code. Verifereum aims to solve this, starting with a verification of the Vyper compiler.
>   
> - **Advancing formal verification on Ethereum:** Verifereum's use of higher-order logic also provides higher reliability and expressivity compared to currently available frameworks based on first-order logic.
>
> - **Limited adoption of formal methods:** Verifereum aims to build a community and provide high-quality documentation and educational resources to onboard more web3 developers to formal verification while bringing formal verification experts to web3.


### Proposed tasks, roadmap and budget?*

*Provide a summary that includes a timeline of the expected work and an estimated budgetary breakdown.*

> ####  Roadmap:
>
> The grant is to fund payroll expenses for the following work.
> 
> - **Formal Specification of a Subset of the Vyper Language (2 months)**:
>   - Develop a definitional interpreter in logic for a subset of the Vyper AST (excluding elements that involve EVM state).
>   - Test the model against the some of the tests developed for the Ivy Vyper AST interpreter (https://github.com/cyberthirst/ivy)
> - **Base Formal Specification of the EVM (1 month)**:
>   - Continue developing our formal specification of the EVM in HOL4 to the extent necessary to support the work on the Vyper definition
>   - Optimize the model for faster execution
>   - Test the model against some of the tests in the Ethereum Test Set (https://github.com/ethereum/tests/)
>
> #### Estimated budget:
> 
> |  Item                  | Timeline | Amount       | Description                                        |
> |------------------------|----------|--------------|----------------------------------------------------|
  > | _Developer Salaries_   | 3 months | $50,000      | Vyper definitional interpreter + minimal EVM model |
> 
> 


### Requested amount

*Choose denominated currency and enter a whole number in the Amount field*

#### Fiat currency*

> USD

#### Amount*

> $50,000

### Why is your project important?*

*Why should solving these problems or addressing these needs be prioritized, what evidence do you have of importance or demand?*

> Smart contract security is paramount to the Ethereum ecosystem, where over 70 million contracts secure hundreds of billions of dollars of value. The blockchain audit industry, currently worth $3 billion is expected to grow tenfold over the next 5 years (https://www.marketsandmarkets.com/PressReleases/blockchain-security.asp), signaling the tremendous demand for rigorous scrutiny of on-chain apps. By mathematically proving that a contract behaves exactly as expected relative to a clearly defined specification, formal verification offers the highest assurance of vulnerability-free code. 
> 
> Despite the strong need and demand for higher safety and formal verification of smart contract applications and compilers, there is still a supply constraint due to a dearth of tooling, educational resources, and qualified practitioners. Verifereum aims to provide a complete and well-documented framework for the formal verification of any Ethereum application while growing an active community of technical and non-technical contributors to foster the adoption of formal methods.


### How does your project differ from similar ones?*

*What other solutions are being worked on, what unique contribution will you make or advance will you provide beyond the state of the art?*

> There are many tools to improve smart contract security (static analysis, fuzzing...). They provide assurance against bugs, but not at the level of formal verification. Formal verification tools like Solidity's SMTChecker work on a high-level language and do not protect against bugs introduced by the compiler. For a contract's binary to be formally verified, its language's compiler itself must be formalized or the compiled binaries must be verified against an EVM specification.
> 
> Formal verification efforts so far, like KEVM or EVM-Dafny, have targeted the latter option. Likewise, the more recent EVM-Vale model in F*/Vale which only handled a subset of the EVM's semantics. Earlier projects gave formal specifications in Isabelle/HOL and CoQ but are not actively used. Work on a Lean model is underway (https://tinyurl.com/drtap9az) but does not fully pass the Ethereum Test Set.
>
> Verifereum solves these approaches' limitations and adds new contributions
> 
> - Compiler verification: Current models target compiled bytecode rather than compilers. By contrast, Verifereum can verify both compilers and compiled code. One of our goals is to fully verify the Vyper compiler.
>
> - Decompilation into logic: Verifereum will offer tooling to decompile EVM bytecode programs into logic, regardless of their original language, to automate verification (https://tinyurl.com/3zbyzpk2). There is nothing similar available for Ethereum applications yet.
>
> - Reliability: Verifereum uses HOL4 which is more trustworthy than the frameworks used by other projects such as K, Dafny, or Vale. HOL4 has been formally proven sound (https://tinyurl.com/mxjb63v3). Its trusted code base is small and extensively reviewed.
> 
> - Expressivity: Unlike K or Dafny which are based on first-order logic, HOL4 is based on higher-order logic which has more expressive semantics (https://philpapers.org/rec/FARTSV), allowing for more complex proofs.
>
> - Depth: HOL4 can be used to prove arbitrarily complex functional correctness properties.


### Describe how your project will result in a public good.*

*Public goods are things like open source code, shared infrastructure, openly shared research, documentation, community building or other benefits provided to the community that are typically under-provided by the free market.*

> Verifereum is fully free and open source. It aims to become the reference framework for formal verification work for all Ethereum applications and to build a large community of contributors. It will contribute to securing the EVM (by providing another formal model of its mechanics), its programming languages such as Solidity and Vyper, and potentially any set of smart contracts. 
> 
> While Verifereum may serve as the basis for for-profit ventures in the future (for instance, auditing or consulting), the formal specifications, research, proofs, and documentation will always remain free and open source. 

### Will your results be open source?*

*If not, please explain why.*

> Yes

### Describe the expected effects of your project proposal on the Ethereum ecosystem.*

*Please list the expected results of the project and explain how they will have a positive effect on the Ethereum ecosystem at large.*

> - **Smart contract security:** Verifereum will enable developers to mathematically prove that their smart contracts are exempt from all exploits of a certain type. This will, in turn, enhance the overall trust in Ethereum as a platform.
> - **Compiler reliability:** The Ethereum ecosystem, with its reliance on a couple of languages with no verified compilers, is particularly vulnerable to compiler bugs. By focusing on compiler verification, starting with Vyper, Verifereum will increase confidence in the correctness of compiled smart contract code.
> - **Advancement of formal methods:** Verifereum will push forward the state-of-the-art in formal verification on Ethereum and provide a more expressive and trustworthy framework for developers to work with.
> - **Community building and education:** Drawing upon the experience and network acquired while building the CakeML community, Verifereum will help grow the pool of developers skilled in formal verification methods. We plan to do so by onboarding technical and non-technical contributors, providing documentation and tutorials, and organizing outreach events. 

### Describe key risks and challenges to your project.*

*What are the critical risks, relating to both project implementation and achieving expected impacts?*

> The main challenges we foresee for Verifereum are:
>
> - **Funding sustainability:** Verifereum aims to be a public good and will need to rely on grant funding in the short term until the product is more mature. There are, however, several ways in which Verifereum can be monetized in the future to ensure the long-term sustainability of the platform.
>   
> - **Maintenance:** Both the EVM and its most popular languages are constantly evolving, which means that our formal models will have to be regularly updated to remain relevant. This process will be labor intensive but can be mitigated by building an active community of contributors and good relationships with compiler developers. For instance, since a formal verification of a compiler provides a significant value add, the compiler team themselves could become directly involved in the maintenance process.
>   
> - **Complexity as an adoption barrier:** Formal verification is inherently complex even for seasoned developers and this may hinder adoption. This is why Verifereum puts a strong emphasis on documentation, education, and community building. Furthermore, the security benefits of formal methods also create a strong incentive for developers to become more familiar with them.


### What are your plans after the grant is completed?*

> We plan on continuing our work on Vyper to expand the definitional interpreter to the whole language, eventually passing the full Ivy test suite. We will then begin work on a formal definition of a Vyper compiler front end, with the long term goal of offering a full formal verification of the compiler. We will also work on completing our EVM model and making sure it passes the whole Ethereum test suite (https://github.com/ethereum/tests?tab=readme-ov-file) 


### If you didn't work on this project, what would you work on instead?*

> If I didn't have support (both collaborators and funding) for Verifereum, I would reconsider my priorities and fall back to other activities including those related to Ethereum staking (e.g. Rocket Pool node operation and community support, non-custodial staking-as-a-service) and those outside of the ecosystem altogether (e.g. activism).

### Have you previously applied to ESP with this same idea or project?*

> No

### Have you applied for or received other funding?*

> No

### Anything else you'd like to share?


> No

### City

*Where are you located, or where is your team located?*

> London

### Country*

> United Kingdom

### Your time zone*

*Please choose your current time zone to help us schedule calls.*

> UTC

### How did you hear about the Ecosystem Support Program?*

Select

### Did anyone recommend that you submit an application to the Ecosystem Support Program?

*Please include the person's name and details of their referral.*
