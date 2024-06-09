# Research + Projects

<style>
  .fluidMedia {
  position: relative;
  padding-bottom: 56.25%; /* proportion value to aspect ratio 16:9 (9 / 16 = 0.5625 or 56.25%) */
  padding-top: 30px;
  height: 0;
  overflow: hidden;
  }

  .fluidMedia iframe {
  position: absolute;
  top: 0; 
  left: 0;
  width: 100%;
  height: 100%;
  }
</style>  
## Contents
- [PL Research / Projects](#pl)
- [Literature Reviews / Independent Studies](#litreviews)
- [Lectures](#lectures)
- [Other Programming Projects](#others)

********************************************************************************
## <a name="pl"></a> PL Research / Projects

### Mica: Automated Differential Testing for OCaml Modules
[(GitHub)](https://github.com/ngernest/mica) [(Documentation)](https://ngernest.github.io/mica/mica/index.html)
- Mica is a tool which automates differential testing for OCaml modules. Mica parses an OCaml module signature and *automatically* generates property-testing code specialized to the interface, checking if two modules
are observationally equivalent. 
- Received Second Prize at the [ICFP'23 Student Research Competition](https://icfp23.sigplan.org/track/icfp-2023-student-research-competition) (Graduate Category)       
([poster](/pdfs/mica_icfp23src_poster.pdf)) ([extended abstract](/pdfs/mica_icfp23src_abstract.pdf))
- Advised by [Harry Goldstein](https://harrisongoldste.in) & Professor [Benjamin Pierce](https://www.cis.upenn.edu/~bcpierce/)
<div align="center" class="fluidMedia">
  <iframe src="/pdfs/mica_icfp23src_poster.pdf" allow="autoplay" frameborder="0">
  </iframe> 
</div>

### Mechanized Type Soundness Proofs for the Hindley-Milner Type System
- Mechanized type soundness proofs for the Hindley-Milner (or "Damas-Milner") type system using the 
[locally nameless representation](https://chargueraud.org/research/2009/ln/main.pdf) in Coq, along with the [LNGen](https://github.com/plclub/lngen) & [Ott](https://github.com/ott-lang/ott) metatheory tools.
- The proofs are for the non-syntax-directed version of the HM type system, as presented in [Peyton Jones et al. (2007)](https://www.microsoft.com/en-us/research/wp-content/uploads/2016/02/putting.pdf).
- Joint work with [Gary Chen](https://www.hanxic.com) & [Zed Wu](https://www.linkedin.com/in/zhiyuan-wu/), advised by Professor [Stephanie Weirich](https://www.cis.upenn.edu/~sweirich/])
- Final project for [CIS 6700](https://github.com/plclub/cis6700-23sp) (Advanced Topics in Programming Languages)
<div align="center" class="fluidMedia">
  <iframe src="/pdfs/6700_report.pdf" allow="autoplay" frameborder="0">
  </iframe> 
</div>

********************************************************************************
## <a name="litreviews"></a> Literature Reviews / Independent Studies

### Survey: Differentially Private Streaming Algorithms
- Discussed the theory of Differential Privacy (DP) and recent work from the algorithm design & PL
literature incorporating DP into streaming algorithms.
- Joint work with [Kavish Shah](https://www.linkedin.com/in/kavishshah15/), advised by Professor [Michael Kearns](https://www.cis.upenn.edu/~mkearns/)
- Final project for [CIS 6250](https://www.cis.upenn.edu/~mkearns/teaching/CIS625/) (Theory of Machine Learning)
<div align="center" class="fluidMedia">
  <iframe src="/pdfs/6250_report.pdf" allow="autoplay" frameborder="0">
  </iframe> 
</div>

### Asymptotic Behavior of Cliques in Inhomogeneous W-random Graphs
[(Report)](/pdfs/urps_report.pdf) [(Slides)](/pdfs/urps_slides.pdf)
- [Hladký et al. (2021)](https://arxiv.org/abs/1903.10570) proved a limit theorem for the no. of cliques in W-random graphs (an inhomogeneous variant of Erdős-Rényi random graphs). In these slides, I introduce the relevant background in graphon theory,
provide a high-level overview of Hladký et al.'s proofs & conduct numerical simulations in Python verifying their results. 
- Independent study, advised by [Anirban Chatterjee](https://statistics.wharton.upenn.edu/profile/anirbanc/#research) & Professor [Bhaswar Bhattacharya](https://statistics.wharton.upenn.edu/profile/bhaswar/)
(via Penn's [Undergraduate Research in Probability & Statistics](https://sites.google.com/view/urps-penn) program)

<div align="center" class="fluidMedia">
  <iframe src="/pdfs/urps_slides.pdf" allow="autoplay" frameborder="0">
  </iframe> 
</div>

### Proving Pólya's Random Walk Theorem using Electric Network Theory
- In these slides, I discuss the applications of electric network theory to 
random walks on integer lattices, focusing on [Doyle & Snell's (1984)](https://math.dartmouth.edu/~doyle/docs/walks/walks.pdf) proof for Pólya's Random Walk Theorem.
- Independent study, advised by [Eric Goodman](https://www.linkedin.com/in/etgoodman) & Professor [Mona Merling](https://www2.math.upenn.edu/~mmerling/)
(via Penn Math's [Directed Reading Program]((https://www2.math.upenn.edu/~tbraz/drp/)))
<div align="center" class="fluidMedia">
  <iframe src="/pdfs/drp_slides.pdf" allow="autoplay" frameborder="0">
  </iframe> 
</div>

********************************************************************************
## <a name="lectures"></a> Lectures

### Programming in the Untyped λ-calculus 
- Slides for a talk I gave for [CIS 6700](https://github.com/plclub/cis6700-23sp) (Advanced Topics in Programming Languages)
- In these slides, I cover the Church & Scott encodings of various datatypes in the untyped λ-calculus,       
following the presentation in Pierce's *Types & Programming Languages* textbook. 
<div align="center" class="fluidMedia">
  <iframe src="/pdfs/6700_lc_slides.pdf" allow="autoplay">
  </iframe> 
</div>

### Parsers in Haskell
- Slides for a guest lecture for [CIS 1940](https://www.seas.upenn.edu/~cis1940/spring23/) (Introduction to Haskell)
- In these slides, I cover monadic parser combinators (à la Parsec), Haskell's `Applicative` typeclass & testing parsers using QuickCheck.
- I also designed an assignment where students build a parser for Lisp-style S-expressions using `Applicative` functors, and test the correctness of their parser using round-trip properties in QuickCheck. 
<div align="center" class="fluidMedia">
  <iframe src="/pdfs/1940_slides.pdf" allow="autoplay" frameborder="0">
  </iframe> 
</div>

********************************************************************************
## <a name="others"></a> Other Programming Projects
### SQL to Pandas Translator 
[(GitHub)](https://github.com/homjason/sql-to-pandas)
<div align="center">     
  <img src="/images/sql_pd.png" alt="sql-to-pandas" width="600" /> 
</div>       

- A tool for translating SQL queries into equivalent Pandas queries, implemented in Haskell.
- I worked on implementing a parser for SQL queries using monadic parser-combinators, 
and verifying the correctness of the parser using QuickCheck. 
- Joint work with [Jason Hom](https://www.linkedin.com/in/homjason), mentored by [Joe Cutler](https://www.cis.upenn.edu/~jwc/)
- Final project for [CIS 5520](https://www.seas.upenn.edu/~cis5520/current/index.html) (Advanced Programming)

### PennOS 
<div align="center">
  <img src="/images/pennos_diagram.png" alt="PennOS" width="800" height="190" /> 
</div>

- A Unix-esque operating system implemented in C (~10k lines of code)
- I worked on the OS kernel, in particular implementing the scheduler and handling signals/process statuses, 
as well as integrating the kernel with the shell. 
- Joint work with [Mati Davis](https://www.linkedin.com/in/mati-davis-816610120), [John Smith](https://www.linkedin.com/in/john-smith-v-71300015b/), [Rohan Verma](https://www.linkedin.com/in/rohanver/?trk=public_profile_browsemap), [Keshav Ramji](https://www.keshavramji.com)
- Final project for [CIS 5480](https://boonloo.cis.upenn.edu/about/teaching/cis548/) (Operating Systems)

### HomeLab
<div align="center">
  <img src="/images/homelab.jpg" alt="homelab" width="600" /> 
</div>

- Custom VPN + Media server, hosted on a PC salvaged from Penn's E-Waste facilities      
- Joint work with [Aaron Shurberg](https://www.linkedin.com/in/aaron-shurberg)     
- Final project for [CIS 1880](https://cis1880.org) (DevOps)   

