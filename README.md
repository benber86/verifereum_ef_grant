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

> Verifereum is a formal model of Ethereum implemented in higher-order logic (HOL4). The project aims to enable the verification of applications and tools within the Ethereum ecosystem, from smart contracts to compilers. Verifereum does not target any specific set of smart contracts or programming languages, but is rather meant to be a general framework for formal verification in the Ethereum space. One of the first projects built on top of Verifereum will be a verification of the Vyper compiler as its clean design and semantics make it a prime candidate for formal modelling.


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
> The grant is to fund payroll expenses for $\color{red}{\textbf{(what would be a reasonable timeline?)}}$ .
> 
> - **Base Formal Specification of the EVM (x months)**:
>   - Draw up an executable formal specification of the EVM in HOL4 
>   - Optimize the model for faster execution
>   - Ensure that the model passes all of the tests in the Ethereum Test Set (https://github.com/ethereum/tests/)
> - **Formal Specification of the Vyper Compiler**:
>   - Draw up a full formal specification of the Vyper AST
>   - Extend the tests for the Ivy Vyper AST interpreter (https://github.com/cyberthirst/ivy) and ensure the model passes them 
>
> #### Estimated budget:
> 
> |  Item                  | Timeline | Amount       | Description                            |
> |------------------------|----------------------------------------|--------------|--------------|
> | _Developer Salaries_  | X |  $50,000       | xxx |
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

> Smart contract security is paramount to the Ethereum ecosystem, where over 70 million contracts secure hundred of billions of dollars of value. The blockchain audit industry, currently worth $3b USD is expected to grow tenfold over the next 5 years (https://www.marketsandmarkets.com/PressReleases/blockchain-security.asp), signalling the tremendous demand for rigorous scrutiny of on-chain apps. By mathematically proving that a contract behaves exactly as expected relative to a clearly defined specification, formal verification offers the highest assurance of vulnerability-free code. 
> 
> Despite the strong need and demand for higher level of safety and formal verification of smart contract applications and compilers, there is still a supply constraint due to a dearth of tooling, educational resources and qualified practicioners. Verifereum aims to provide a complete and well-documented framework for the formal verification of any Ethereum application while growing an active community of technical and non-technical contributors to foster the adoption of formal methods.


### How does your project differ from similar ones?*

*What other solutions are being worked on, what unique contribution will you make or advance will you provide beyond the state of the art?*

> There are many tools available to help Ethereum smart contract developers improve the security of their code. Tools for static analysis, fuzzing or mutation testing all provide additional assurance against bugs and vulnerabilities, but not at the level provided by formal verification. On the other hand, formal verification is more complex, labor-intensive and has comparatively less smart-contract specific tooling. There are verification tools such as Solidity's SMTChecker (https://docs.soliditylang.org/en/latest/smtchecker.html), solc-verify (https://github.com/SRI-CSL/solidity) or VeriSol (https://github.com/microsoft/verisol) but they work directly on a high level programming language and do not offer security guarantees against bugs introduced by the compiler. For a contract's binary to be formally verified, either its language's compiler itself must be formalized or the post-compilation binaries must be verified against an EVM specification.
>
> Most formal verification efforts so far have targeted the latter option. KEVM (https://ieeexplore.ieee.org/document/8429306) by Runtime Verification and EVM-Dafny (https://github.com/Consensys/evm-dafny) by Consensys have been under development since 2018 and 2022 respectively and are currently the most widely used frameworks. Both provide executable formal specifications of the EVM that can be used to formally verify contracts at the bytecode level. More recently, EVM-Vale (https://link.springer.com/chapter/10.1007/978-981-97-0006-6_3) offered a formal model of the EVM in F*/Vale which could be used to formally verify bytecode programs. The authors, however, only worked with a subset of the EVM's semantics. Earlier projects tried to give formal specification in Isabelle/HOL (https://github.com/pirapira/ethereum-formal-verification-overview) and CoQ (https://arxiv.org/abs/1810.04828) but are not actively used or maintained. Work on a Lean model is under way (https://github.com/NethermindEth/EVMYulLean) but remains in infancy and does not fully pass the Ethereum Test Set. 
> 
> These approaches, however, all have their own limitations which Verifereum aims to overcome while offering a unique new contributions. 
The main points on which Verifereum differentiates itself from existing solutions are:
> 
> - Reliability: Verifereum uses HOL4 which is demonstrably more trustworthy than the frameworks used by currently available projects such as K, Dafny or Vale. HOL4 has been formally proven sound (https://www.cl.cam.ac.uk/~jrh13/papers/holhol.html, https://www.cst.cam.ac.uk/news/ramana-kumar-wins-acm-sigplan-doctoral-dissertation-award) and its trusted code base (the "kernel") is both extremely small and extensively reviewed. Furthermore, HOL4 can produce independently checkable proofs (in OpenTheory format).
>   
> - Expressivity: Unlike K or Dafny which are based in first-order logic, HOL4 is based on higher order logic whose semantics are much more expressive (https://philpapers.org/rec/FARTSV). This allows for more complex and comprehensive proofs, beyond simple assertions about a contract's expected behavior.
> 
> - Depth: Because of the above, HOL4 can be used to prove arbitrarily complex functional correctness properties.
> 
> - Compiler verification: All current models target post-compilation bytecode rather than compilers. And while there have been a few attempts to formalize the semantics of Solidity (https://doi.org/10.1007/978-3-030-92124-8_23, . https://doi.org/10.1007/978-3-030-03592-1_13), the work remains lacunary. By contrast, Verifereum aims to be a framework with which both compilers and compiled code can be verified, leveraging the experience, community and knowledge gained from building CakeML, a fully verified compiler for the ML programming language. The first project built on Verifereum is a verified version of the Vyper compiler, with the view to support additional languages in the future.
>
> - Decompilation into logic: Verifereum will offer tooling to automatically decompile EVM bytecode programs, regardless of their original high level language, into logic to facilitate and automate verification (https://www.cl.cam.ac.uk/~mom22/decompilation/)



### Describe how your project will result in a public good.*

*Public goods are things like open source code, shared infrastructure, openly shared research, documentation, community building or other benefits provided to the community that are typically under-provided by the free market.*

> Verifereum is fully free and open source. It aims to become the reference framework for formal verification work for all Ethereum applications and to build a large community of contributors. It will contribute to secure the EVM (by providing another formal model of its mechanics), its programming languages such as Solidity and Vyper, and potentially any set of smart contracts. 
> 
> While Verifereum may serve as the basis for for-profit ventures in the future (for instance, auditing or consulting), the formal specifications, research, proofs and documentation will always remain free and open source. 

### Will your results be open source?*

*If not, please explain why.*

> Yes

### Describe the expected effects of your project proposal on the Ethereum ecosystem.*

*Please list the expected results of the project and explain how they will have a positive effect on the Ethereum ecosystem at large.*

> - **Improve security:** By offering an alternative to Solidity's current monopoly, Vyper reduces the systemic risk associated with relying on a single language and provides developers with more options tailored to their needs and expertise.
> - **:** Vyper's design principles prioritize security and audibility. Vyper is well integrated with security analysis tools like Slither and Echidna and offers automated fuzzing via Titanoboa, making it easier for developers to create and verify secure smart contracts.
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

> $\Huge{\color{red}{\textbf{For Ramana to fill out}}}$


### If you didn't work on this project, what would you work on instead?*

> $\Huge{\color{red}{\textbf{For Ramana to fill out}}}$

### Have you previously applied to ESP with this same idea or project?*

> No

### Have you applied for or received other funding?*

> No

### Anything else you'd like to share?


> $\Huge{\color{red}{\textbf{For Ramana to fill out}}}$

### City

*Where are you located, or where is your team located?*

### Country*

> United States

### Your time zone*

*Please choose your current time zone to help us schedule calls.*

> $\Huge{\color{red}{\textbf{For Ramana to fill out}}}$

### How did you hear about the Ecosystem Support Program?*

Select

### Did anyone recommend that you submit an application to the Ecosystem Support Program?

*Please include the person's name and details of their referral.*
