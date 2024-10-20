# Verifereum 
### First name*

> Ramana

### Last name*

> Kumar

*This should be the main contact we'll be talking to.*

### Email*

> $\Huge{\color{red}{\textbf{For Ramana to fill out}}}$


### Organization name*

*Name of your team or organization. If you do not have an organization name, write "N/A".*

> Verifereum

### Team profile*

*Briefly describe your organization. Provide links to previous work. How is your organization suited to the project's objectives, and how does it provide the necessary expertise?*

> Verifereum is currently led by Ramana Kumar. Ramana has a PhD in computer science and has done extensive academic research on formal verification (https://scholar.google.com/citations?user=OyX1-qYAAAAJ&hl=en&oi=sra). They are a world leading expert on compiler verification and a key contributor to CakeML, a verified implementation of ML and one of a handful of formally verified compilers. An active contributor to the liquid staking derivative ecosystem on Ethereum, Ramana combines their expertise in formal verification with a deep knowledge of the EVM. His background makes him uniquely qualified to build Verifereum, an EVM formal verification framework and Verifereum-based compiler verification projects.
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

> Verifereum .

### Project repo

*GitHub or other public repository of the project or related work.*

> [https://github.com/verifereum](https://github.com/verifereum)


### Project category*

*Please choose a category that your project best fits in.*

> Formal Verification

### Brief project summary*

*Describe your project in a few sentences (you'll have the chance to go into more detail in the long form). If it's already underway, provide links to any existing published work.*

> Verifereum is a formal model of Ethereum implemented in higher-order logic (HOL4). The project aims to enable the verification of applications and tools within the Ethereum ecosystem, from smart contracts to compilers. Verifereum does not target any specific set of smart contracts or programming languages, but is rather meant to be a general framework for formal verification efforts in the Ethereum space. One of the first projects built on top of Verifereum will be a verification of the Vyper compiler as its clean design and semantics make it a prime candidate for formal modelling.


### Describe the current status of the project and progress achieved so far*

*For example, do you have an MVP? Please describe its functionality and limitations and provide a link to it here.*

> Verifereum already has a basic formal model of the EVM in HOL4, available at https://github.com/verifereum/verifereum. While not fully complete, the model is executable $\color{red}{\textbf{(is it already?)}}$ and currently passes some $\color{red}{\textbf{(proportion?)}}$ tests from the Ethereum Test Set (https://github.com/ethereum/tests). Work towards a definitional interpreter targeting the Vyper compiler has also started by formalizing the language's Abstract Syntax Tree (AST) at https://github.com/xrchz/vyper-hol/tree/main. The current formalization is still at an early stage but covers basic types, expressions, and control flow constructs.


### What problem(s) are being solved by within the scope of the grant?*

*What is the specific problems, research questions, or needs you are trying to address?*

> - ???
> - ???
> - ???


### Proposed tasks, roadmap and budget?*

*Provide a summary that includes a timeline of the expected work and an estimated budgetary breakdown.*

> ####  Roadmap:
>
> The grant is to fund security and payroll expenses for 1 year to allow Vyper to implement new features and optimizations in a fully secure way while improving tooling and developer experience.
> 
> - **Language Features**:
>   - Built-in for proxies (4 months)
>   - Improvements and fixes for the decimal type (2 months)
>   - New type for assets (3 months)
>   - Structs (3 months)
>   - Generics (6 months to a year)
>   - Traits (6 months to a year)
> - **Compiler Optimizations**:
>   - Implementing better constant propagation and dead code elimination through sparse conditional constant propagation (1 year, continuous).
>   - Fully phase out the old intermediate representation and replace it with the new Venom (1 year, continuous)
>   - Improve existing optimizations: algebraic and branch optimization, stack reordering, etc. (1 year, continuous)
> - **Auditing**: Ensure every new major release is fully reviewed by multiple auditors (1 year, continuous)
> - **Compiler Correctness**: Test the correctness of the Vyper compiler by
>   - Developing a definitional interpreter to serve as the language specification (3 months)
>   - Creating a Vyper program generator to automatically generate semantically valid contracts (2 months)
>   - Using the interpreter as a fuzzing oracle to assert that the execution of the compiled bytecode has the same outputs as the interpreted contract (1 month)
>   - Building a framework on top of the Abstract Syntax Tree (AST) and Venom Intermediary Representatoin using lattices and control flow & data flow analyses (6 months)
> - **Tooling**: Improve the Titanoboa interpreter and work on the development of the new Gaboon framework by:
>   - Improving network management and cross-chain features (1 month)
>   - Adding deployment history and log management features (1 month)
>   - Offering secure keystores and account management (1 month)
>   - Project and module management via CLI (1 month)
>   - Console feature to quickly load and interact with contracts (2 months)
>   - Vyper REPL (2 months)
>   - Improvements to Titanoboa documentation, Gaboon documentation and tutorial videos (2 months)
>
> #### Estimated budget:
> 
> |  Item                  | Timeline | Amount       | Description                            |
> |------------------------|----------------------------------------|--------------|--------------|
> | _Security & Auditing_  | 1 year, continuous |  $1,212,000       | Vyper's yearly auditing budget currently sits at $1,012,000 to work with three auditors (Chain Security, Statemind, OtterSec) and perform reviews of every new Vyper release as well as continuous improvement to the codebase security. We budget another $200,000 to hire an external auditor on a contractual basis and a full-time security engineer to test the correctness of the Vyper compiler through differential fuzzing and abstract analysis. |
> | _Developer Salaries_         | 1 year, continuous | $1,320,000 | The budget would cover the salary for Vyper's Lead Developer (Charles Cooper), one Senior Developer (Harry Kalogirou, FT) and one Junior Developer (Adam) - all on a full time basis. It also includes the salaries of an additional compiler engineer and one senior developer to work on Titanoboa and tooling, both on also on a full time basis |
> | **Total** | **1 year** | **$2,532,000** | |
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

Smart contract security is absolutely paramount to Ethereum where 70 million contracts secure hundred of billions of dollars of value. The blockchain audit industry, currently worth $3b USD is expected to grow tenfold over the next 5 years (https://www.marketsandmarkets.com/PressReleases/blockchain-security.asp), signalling the tremendous demand for rigorous scrutiny of on-chain apps. By mathematically proving that a contract behaves exactly as expected relative to a clearly defined specification, formal verification offers the highest assurance of vulnerability-free code. 

Despite the strong need and demand for higher level of safety and formal verification of smart contract applications and compilers, there is still a supply constraint due to a dearth of tooling, educational resources and qualified practicioners. Verifereum aims to provide a complete and well-documented framework for the formal verification of any Ethereum application while growing an active community of technical and non-technical contributors to foster the adoption of formal methods.


### How does your project differ from similar ones?*

*What other solutions are being worked on, what unique contribution will you make or advance will you provide beyond the state of the art?*

There are many tools available to help Ethereum smart contract developers improve the security of their code. Tools for static analysis, fuzzing or mutation testing all provide additional assurance against bugs and vulnerabilities, but not at the level provided by formal verification. On the other hand, formal verification is more complex, labor-intensive and has comparatively less smart-contract specific tooling. There are verification tools such as Solidity's SMTChecker (https://docs.soliditylang.org/en/latest/smtchecker.html), solc-verify (https://github.com/SRI-CSL/solidity) or VeriSol (https://github.com/microsoft/verisol) but they work directly on a high level programming language and do not offer security guarantees against bugs introduced by the compiler. For a contract's binary to be formally verified, either its language's compiler itself must be formalized or the post-compilation binaries must be verified against an EVM specification.

Most formal verification efforts so far have targeted the latter option. KEVM (https://ieeexplore.ieee.org/document/8429306) by Runtime Verification and EVM-Dafny (https://github.com/Consensys/evm-dafny) by Consensys have been under development since 2018 and 2022 respectively and are currently the most widely used frameworks. Both provide executable formal specifications of the EVM that can be used to formally verify contracts at the bytecode level. More recently, EVM-Vale (https://link.springer.com/chapter/10.1007/978-981-97-0006-6_3) offered a formal model of the EVM in F*/Vale which could be used to formally verify bytecode programs. The authors, however, only worked with a subset of the EVM's semantics. Earlier projects tried to give formal specification in Isabelle/HOL (https://github.com/pirapira/ethereum-formal-verification-overview) and CoQ (https://arxiv.org/abs/1810.04828) but are not actively used or maintained. Work on a Lean model is under way (https://github.com/NethermindEth/EVMYulLean) but remains in infancy. 

These approaches, however, all have their own limitations which Verifereum aims to overcome while offering a unique new contributions.


There have been a few other attempts to draw up formal specifications of the EVM which can be use for verification, however not all are actively maintained or usable and those that are have their own limitations and drawbacks. Verifereum also targets a much wider scope for verification compared to currently available solutions. The two most advanced formal verification frameworks currently available also only target EVM bytecode verification, 

- , and bytecode verification is unpractical for large or complex contracts. Furthermore, the author identified several limitations with the F*/Vale framework itself, including a restrictive type system, slow verification speed and lack of support and documentation.

While there have been a number of 
> Vyper's main competitors are other EVM smart contract programming languages such as Solidity, Yul, Fe, and Edge. Vyper differs by its focus on readability, security and simplicity:
> - Vyper is a high level (unlike Yul) language. It is entirely production ready (unlike Fe or Edge) and does not suffer from "stack too deep" errors (unlike Solidity).
> - Vyper is designed to make contracts maximally human readable, which translates into a direct reduction (-20% according to auditors) of the time and costs of auditing compared to Solidity.
> - Vyper's highly optimized backend (Venom) allows the language to offer high-level syntax with the performance of a low-level language like Yul. Benchmarks show that compiled Vyper contracts perform on par or better than highly optimized Solidity contracts from the Solmate or Solady libraries on gas costs and bytecode size. 
> - Vyper takes an opinionated approach to safety and enforces code correctness by removing the main security pitfalls of Solidity (operator and function overloading, recursive calls, class inheritance, inline assembly, etc.)
> - Vyper's simple, pythonic syntax, its tight-knit and supportive community, and its steadily improving, user friendly tooling make the language uniquely positioned to attract new web3 developers.

### Describe how your project will result in a public good.*

*Public goods are things like open source code, shared infrastructure, openly shared research, documentation, community building or other benefits provided to the community that are typically under-provided by the free market.*

> Vyper is fully free and open source, released under a permissive Apache license. We provide key infrastructure on top of which some of the major building blocks of Ethereum's DeFi (Curve, Yearn, Lido) have been built, producing billions of dollars of value for the ecosystem. 
> 
> Like all smart contract programming languages, Vyper is ill-suited to market based funding. On one hand, mechanisms to fund development by charging for usage (for instance by redirecting some of the gas fees to fund compiler development) increase costs for users and risk lowering adoption. They can also cause conflicts over fee split between compiler developers and smart contract developers, and create perverse incentives (gas guzzling, savage forking, wash trading). On the other hand, private funding threatens the neutrality of the language and puts it under the tutelage of its financial backers. 

### Will your results be open source?*

*If not, please explain why.*

> Yes

### Describe the expected effects of your project proposal on the Ethereum ecosystem.*

*Please list the expected results of the project and explain how they will have a positive effect on the Ethereum ecosystem at large.*

> - **Improve language diversity:** By offering an alternative to Solidity's current monopoly, Vyper reduces the systemic risk associated with relying on a single language and provides developers with more options tailored to their needs and expertise.
> - **Improve smart contract security:** Vyper's design principles prioritize security and audibility. Vyper is well integrated with security analysis tools like Slither and Echidna and offers automated fuzzing via Titanoboa, making it easier for developers to create and verify secure smart contracts.
> - **Increase Ethereum's developer base:** Vyper's pythonic syntax lowers the entry barrier for web2 developers familiar with Python, potentially attracting a new cohort of developers to Ethereum. Vyper implements all of the main features that developers expect from a smart contract programming language, while tools like Titanoboa and Gaboon offer fast testing and debugging capacities, further enhancing developer experience and making Ethereum development more accessible.
> - **An alternative intermediate representation (IR) to Yul for future EVM languages:** Venom, Vyper's intermediate representation, could serve as an alternative to Yul for future smart contract languages, further fostering innovation and diversity in Ethereum's language ecosystem. 

### Describe key risks and challenges to your project.*

*What are the critical risks, relating to both project implementation and achieving expected impacts?*

> One of the main risks and challenges facing Vyper today is ensuring sustainable funding to grow a dedicated core team of high quality developers over the long term. Vyper relies solely on grants whose outcomes are not easily predictable and development can be stalled due to lack of funding.
> 
> Adoption also remains a key challenge. While Vyper has seen increased interest, it still lags behind Solidity in terms of developer mindshare and ecosystem support. Convincing developers to switch or learn a new language can be difficult, even with Vyper's advantages and more outreach and community building efforts are needed to onboard the next generation of web3 devs to Vyper.
> 
> Lastly, there are risks inherent to maintaining a rapid pace of development in the highly adversarial context of smart contracts. As the language and its ecosystem grow, thorough auditing and testing become increasingly complex, costly and time-consuming.


### What are your plans after the grant is completed?*

> Continue to work on improving Vyper and its tooling and grow our community of developers until we are the first programming language on the EVM.

### If you didn't work on this project, what would you work on instead?*

> $\Huge{\color{red}{\textbf{For Ramana to fill out}}}$

### Have you previously applied to ESP with this same idea or project?*

> No

### Have you applied for or received other funding?*

> No

### Anything else you'd like to share?


> $\Huge{\color{red}{\textbf{For Charles to fill out}}}$

### City

*Where are you located, or where is your team located?*

### Country*

> United States

### Your time zone*

*Please choose your current time zone to help us schedule calls.*

> $\Huge{\color{red}{\textbf{For Charles to fill out}}}$

### How did you hear about the Ecosystem Support Program?*

Select

### Did anyone recommend that you submit an application to the Ecosystem Support Program?

*Please include the person's name and details of their referral.*
