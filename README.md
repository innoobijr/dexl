# DEXL: a compositional language for designing DeX experiments


#### dexl is an interpreted langauge written in Rust. a dexl program is an experiment. there are specific types of statements 
#### in an experiment defintion language. allows branching dexl core allows interacting the the dexl registry. 
#### fully fledge programming environment for defining and describing experiments. 
#### an expression evaluates to a notebook, a catalog, a collector, or a base tpyes
#### the dexl store capture this information for an experiment. 
#### there is no notion of local scope. There is only a global scope. We will consider adding funcitons later.
#### We have a minimal experiment definition language with its corresponding verifier. 
#### each dexl object has a corresponding generator for it rosette equivalent. This means for every dexl program we can pass its description to 
#### rosette for solving. Every call to solve transpiles dexl to rosette. Verification is encoded in Rosette and the specification (dexl) is 
#### is checked against that constraints in Rosette. 
#### in this case, I have a between-subjects designing, but assign only one treatment to a user. DEXL-verifiers informs me that I'mviolated the asummptions of a between subjects designing.
#### the a compiler can hardened a shit program, we would like to youse dexl to synthesize robust and well-powered experiments. power is just a min constraint, powered with correction change the value minimized. Executed from code that result an int and solves with that integer


## Introduction



### Key Components
1. Collector
2. Notebook
3. Challenge
4. Resources
5. Catalog


