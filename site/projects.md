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
- [Research / Projects](#projects)
- [Presentations / Lectures](#lectures)
- [Other Programming Projects](#others)

********************************************************************************
## <a name="projects"></a> Research / Projects

### Chamelean: Property-Based Testing for Lean via Metaprogramming
[(GitHub)](https://github.com/ngernest/chamelean)
- Chamelean is an extension of Lean's [Plausible](https://github.com/leanprover-community/plausible) property-based testing (PBT) library, which takes user-defined inductive relations and automatically derives specialized random generators, enumerators and checkers
- I used Lean's [metaprogramming facilities](https://leanprover-community.github.io/lean4-metaprogramming-book/) to implement algorithms used by Rocq's [QuickChick](https://github.com/QuickChick/QuickChick) PBT framework to compile inductive relations into correct-by-construction PBT generators
  - For details, see these papers from [POPL '18](https://dl.acm.org/doi/10.1145/3158133) & [PLDI '22](https://dl.acm.org/doi/10.1145/3519939.3523707)
- Work done during an internship at Amazon Web Services, advised by [Mike Hicks](https://mhicks.me) & [Cody Roux](https://www.kleene.church), with collaborators at [UMD](https://plum-umd.github.io) ([Segev Elazar Mittelman](https://www.linkedin.com/in/segevem/), [Harry Goldstein](https://harrisongoldste.in) & [Leo Lampropoulos](https://lemonidas.github.io))

<div align="center" class="fluidMedia">
  <iframe src="/pdfs/chamelean_public_slides.pdf" allow="autoplay" frameborder="0">
  </iframe> 
</div>

### Mica: Automated Differential Testing for OCaml Modules
[(OCaml Workshop '24 paper)](/pdfs/ocaml24_mica.pdf) [(ICFP '23 SRC poster)](/pdfs/mica_icfp23src_poster.pdf) [(GitHub)](https://github.com/ngernest/mica) [(Web demo)](https://ngernest.github.io/mica/demo)
- Mica is a PPX compiler extension which automates differential testing for OCaml modules. Mica *automatically* generates property-testing code specialized to the interface, checking if two modules are observationally equivalent. 
- Available to [install via Opam](https://opam.ocaml.org/packages/ppx_mica/)
- Presented paper at the [OCaml Workshop 2024](https://icfp24.sigplan.org/home/ocaml-2024#About) (co-located with ICFP '24)
- Received Second Prize at the [ICFP '23 Student Research Competition](https://icfp23.sigplan.org/track/icfp-2023-student-research-competition)     
- Advised by [Harry Goldstein](https://harrisongoldste.in) & [Benjamin Pierce](https://www.cis.upenn.edu/~bcpierce/)
<div align="center" class="fluidMedia">
  <iframe src="/pdfs/ocaml24_mica.pdf" allow="autoplay" frameborder="0">
  </iframe> 
</div>

### Verified Brzozowski and Antimirov Derivatives 
[(GitHub)](https://github.com/ngernest/regexes)
- Mechanized Coq proofs about the equivalence of [Brzozowski derivatives](https://harrisongoldste.in/languages/2017/09/30/derivatives-of-regular-expressions.html), [Antimirov derivatives](https://semantic-domain.blogspot.com/2013/11/antimirov-derivatives-for-regular.html), and their [zipper](https://en.wikipedia.org/wiki/Zipper_(data_structure)) representation ([Edelmann 2020](https://infoscience.epfl.ch/server/api/core/bitstreams/4fcb9f0f-7ac1-484f-823c-c19de39dd9ff/content))
- Implemented executable derivative-based regex matchers in OCaml, tested using QuickCheck
- Joint work with [Laura Zielinski](https://www.linkedin.com/in/lauraczielinski/), advised by [Jules Jacobs](https://julesjacobs.com) and [Nate Foster](https://www.cs.cornell.edu/~jnfoster/)
- Final project for [CS 6115](https://www.cs.cornell.edu/courses/cs6115/2024fa/) (Certified Software Systems)
<div align="center" class="fluidMedia">
  <iframe src="/pdfs/6115_project_slides.pdf" allow="autoplay" frameborder="0">
  </iframe> 
</div>

### Flattening the Bril Intermediate Representation
[(GitHub)](https://github.com/ngernest/flat-bril) [(Blog post)](https://www.cs.cornell.edu/courses/cs6120/2025sp/blog/flat-bril/)            
<div align="center">     
  <img src="/images/flat_bril_graph.png" alt="flat-bril-performance-graph" width="800" /> 
</div>    

- More details in the [blog post](https://www.cs.cornell.edu/courses/cs6120/2025sp/blog/flat-bril/) about this project! 
- Used Rust to implement a [flattened](https://www.cs.cornell.edu/~asampson/blog/flattening.html) representation for the [Bril IR](https://capra.cs.cornell.edu/bril/) & an interpreter that works natively over the flattened representation
- Joint work with [Sam Breckenridge](https://www.linkedin.com/in/samuel-breckenridge-4729b719a/) and [Katherine Wu](https://katherinewu312.github.io), advised by [Adrian Sampson](https://www.cs.cornell.edu/~asampson/)
- Final project for [CS 6120](https://www.cs.cornell.edu/courses/cs6120/2025sp/) (Advanced Compilers)

### Mechanized Type Soundness Proofs for the Hindley-Milner Type System
- Mechanized type soundness proofs for the Hindley-Milner (or "Damas-Milner") type system using the 
[locally nameless representation](https://chargueraud.org/research/2009/ln/main.pdf) in Coq, along with the [LNgen](https://github.com/plclub/lngen) & [Ott](https://github.com/ott-lang/ott) metatheory tools.
- The proofs are for the non-syntax-directed version of the HM type system, as presented in [Peyton Jones et al. (2007)](https://www.microsoft.com/en-us/research/wp-content/uploads/2016/02/putting.pdf).
- Joint work with [Gary Chen](https://www.hanxic.com) & [Zed Wu](https://www.linkedin.com/in/zhiyuan-wu/), advised by [Stephanie Weirich](https://www.cis.upenn.edu/~sweirich/])
- Final project for [CIS 6700](https://github.com/plclub/cis6700-23sp) (Advanced Topics in Programming Languages)
<div align="center" class="fluidMedia">
  <iframe src="/pdfs/6700_report.pdf" allow="autoplay" frameborder="0">
  </iframe> 
</div>

********************************************************************************
## <a name="lectures"></a> Lectures

### seL4 : Formal Verification of an OS Kernel (Paper Presentation)
- Slides for a paper presentation I gave for [CS 6410](https://www.cs.cornell.edu/courses/cs6410/2025fa/home.html) (Advanced Systems) 
- In these slides, I present [Klein et al's (SOSP 2009)](https://dl.acm.org/doi/10.1145/1629575.1629596) paper on the seL4 operating system and its role in the history of formally-verified OSes
<div align="center" class="fluidMedia">
  <iframe src="/pdfs/sel4_slides.pdf" allow="autoplay">
  </iframe> 
</div>

### Programming in the Untyped λ-calculus 
- Slides for a talk I gave for [CIS 6700](https://github.com/plclub/cis6700-23sp) (Advanced Topics in Programming Languages)
- In these slides, I cover the Church & Scott encodings of various datatypes in the untyped λ-calculus,       
following the presentation in Pierce's *Types & Programming Languages* textbook. 
<div align="center" class="fluidMedia">
  <iframe src="/pdfs/6700_lc_slides.pdf" allow="autoplay">
  </iframe> 
</div>

### Parsers in Haskell
[(GitHub)](https://github.com/ngernest/parser-combinator-class)    
- Slides for a guest lecture for [CIS 1940](https://www.seas.upenn.edu/~cis1940/spring23/) (Introduction to Haskell)
- In these slides, I cover monadic parser combinators (à la Parsec), Haskell's `Applicative` typeclass & testing parsers using QuickCheck.
- I also designed an [assignment](https://github.com/ngernest/parser-combinator-class) where students build a parser for Lisp-style S-expressions using `Applicative` functors, and test the correctness of their parser using round-trip properties in QuickCheck. 
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
- I worked on implementing a parser for SQL queries using monadic parser combinators, 
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
