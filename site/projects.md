# Research + Projects
## Contents
- [PL research / projects](#pl)
- [Literature reviews](#litreviews)
- [Lectures](#lectures)
- [Other programming projects](#others)

********************************************************************************
## [PL research / projects](#pl)

### Mica: Automated Property-Based Testing for OCaml Modules [(GitHub)](https://github.com/homjason/sql-to-pandas) [(Documentation)](https://ngernest.github.io/module_pbt/module_pbt/index.html)
- A tool which parses an OCaml module signature and automatically generates 
property-testing code specialized to the interface, checking if two modules
implementing the interface are observationally equivalent. 
- Advised by Prof. Benjamin Pierce & Harry Goldstein

### Mechanized Type Soundness Proofs for the Hindley-Milner Type System
- We mechanized type soundness proofs for the Hindley-Milner type system using the 
locally nameless representation in Coq, using the LNGen & Ott metatheory tools
- We focused on the non-syntax-directed version of the HM type system, as presented in [*Practical Type Inference for Arbitrary-Rank Types*](https://www.microsoft.com/en-us/research/wp-content/uploads/2016/02/putting.pdf) (Peyton Jones et al. 2007)
- Joint work with Gary Chen & Zed Wu, advised by Prof. Stephanie Weirich
- Final project for CIS 6700 (Advanced Topics in Programming Languages)
<div align="center">
  <iframe src="/pdfs/6700_report.pdf" width="640" height="480" allow="autoplay" >
  </iframe> 
</div>

********************************************************************************
## [Literature Reviews](#litreviews)

### Survey: Differentially Private Streaming Algorithms
- Joint work with Kavish Shah, advised by Prof. Michael Kearns
- Final project for CIS 6250 (Theory of Machine Learning)
<div align="center">
  <iframe src="/pdfs/6250_report.pdf" width="640" height="480" allow="autoplay" >
  </iframe> 
</div>

### Asymptotic Behavior of Cliques in Inhomogeneous W-random Graphs
- Independent study, advised by Prof. Bhaswar Bhattacharya & Anirban Chatterjee        
(via Penn's Undergraduate Research in Probability & Statistics program)
<div align="center">
  <iframe src="/pdfs/urps_slides.pdf" width="640" height="480" allow="autoplay" >
  </iframe> 
</div>

### Proving Pólya's Random Walk Theorem using Electric Network Theory
- Independent study, advised by Eric Goodman         
(via Penn's Directed Reading Program)
<div align="center">
  <iframe src="/pdfs/drp_slides.pdf" width="640" height="480" allow="autoplay" >
  </iframe> 
</div>

********************************************************************************
## [Lectures](#lectures)

### Programming in the Untyped λ-calculus 
- Lecture for CIS 6700 (Advanced Topics in Programming Languages)
- Covered Church & Scott encodings of various datatypes in the untyped λ-calculus
<div align="center">
  <iframe src="/pdfs/6700_lc_slides.pdf" width="640" height="480" allow="autoplay" >
  </iframe> 
</div>

### Parsers in Haskell
- Guest lecture for CIS 1940 (Introduction to Haskell)
- Covered monadic parser combinators, the `Applicative` typeclass & testing parsers         
using round-trip properties in QuickCheck 
<div align="center">
  <iframe src="/pdfs/1940_slides.pdf" width="640" height="480" allow="autoplay" >
  </iframe> 
</div>

********************************************************************************
## [Other programming projects](#others)
### [SQL to Pandas Translator](https://github.com/homjason/sql-to-pandas)   
<div align="center">     
  <img src="/images/sql_pd.png" alt="sql-to-pandas" width="600" /> 
</div>       

- A tool for translating SQL queries into equivalent Pandas queries, implemented in Haskell.
- I worked on implementing a parser for SQL queries using monadic parser-combinators, 
and verifying the correctness of the parser using QuickCheck. 
- Joint work with Jason Hom, mentored by Joe Cutler 
- Final project for CIS 5520 (Advanced Programming)

### PennOS 
<div align="center">
  <img src="/images/pennos_diagram.png" alt="PennOS" width="800" height="190" /> 
</div>

- A Unix-esque operating system implemented in C (~10k lines of code)
- I worked on the OS kernel, in particular implementing the scheduler and handling signals/process statuses, 
as well as integrating the kernel with the shell. 
- Joint work with Mati Davis, John Smith, Rohan Verma, Keshav Ramji
- Final project for CIS 5480 (Operating Systems)

### [HomeLab](https://docs.google.com/presentation/d/1fL55MLWr2VaVK5deRYRwu6vWKUUKeHCSRbeT5pGzqGA/edit?usp=sharing)
- Custom VPN + Media server, hosted on a PC salvaged from Penn's E-Waste facilities
- Joint work with Aaron Shurberg
- Final project for CIS 1880 (DevOps)

