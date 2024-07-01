# Dragan's Commit Notation and Most Used Shortcuts


### Commit notation
**Heuristic**: Keep commit messages short in order to reduce the relative cost of committing, which means you’ll commit more often.  
Make use of the `⌘`+`K`, `⌘`+`⏎`/`⌘`+`⌥`+`K` shortcuts in IntelliJ IDE to move to the commit window and commit/push.

#### Rename
- `rm` - rename method  
- `rv` - rename variable  
- `rp` - rename parameter  
- `rf` - rename field

#### Extract
- `xm` - extract method  
- `xp` - extract parameter  
- `xv` - extract variable  
- `xf` - extract field  
- `xc` - extract constant  
- `xC` - extract class  

#### Inline
- `iv` - inline variable  
- `im` - inline method  
- `ip` - inline parameter  

#### Move
- `mm` - move method  
- `tda` - Tell Don’t Ask
- `fmt` - format  
- `rd` - remove duplication  


_**Every change commited must be deployable to production. If a commit is not deployable, the change is most likely not sufficiently small. Find smaller step instead.**_  
If anyone in the group is feeling anxious about the risk of the change (they feel a change is too risky), we revert back to safety and do it in smaller, safer steps. Anxiety about the step is useful feedback about the risk and size of the change. That is especially important in code that is not covered with tests or that we need to tweak enough to be able to test it (catch 22).


### Most Used Shortcuts

#### Refactorings  
- Rename method - `Shift` + `F6`  
- Extract variable - `Command` + `Option` + `V`  
- Extract method - `Command` + `Option` + `M`  
- Extract field (convert a local variable to a class field) - `Command` + `Option` + `F`  
- Extract constant - `Command` + `Option` + `C`
- Inline variable/method - `Command` + `Option` + `N`  
- Extract parameter - `Command` + `Option` + `P`  

- Change method signature - `Command` + `F6`  
- Move static method - `F6`  
- Magic shortcut! Move a static method to a class of one of the parameter's and make it an instance method (also called Make Method Non-Static) - `Command` + `Option` + `I`  

- Format code - `Command` + `Option` + `L`  

#### Commit and Push  
- Commit - `Command` + `K`  
- Push - `Command` + `Shift` + `K`
- Commit and push - `Command` + `Option` + `K`  
- Discard not committed changes - `Command` + `Option` + `Z`

#### Tests  
- Run all tests in solution - `Command` + `;` + `L`  
- Run last test session - `Command` + `;` + `Y`  
- Run all tests with coverage - `Command` + `;` + `K`  

#### Code Navigation and Selection  
- Go to method definition/find usages - `Command` + `B`
- Expand selection - `Option` + `Up`  
- Shrink selection - `Option` + `Down`  
- Move line/code block/method up/down - `Command` + `Shift` + `Up`/`Down`  
