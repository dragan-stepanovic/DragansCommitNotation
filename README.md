# Dragan's Commit Notation and Most Used Shortcuts


### Commit notation
**Heuristic**: Keep commit messages short in order to reduce the relative cost of committing, which means you’ll commit more often.  
Make use of the `⌘`+`K`, `⌘`+`⏎`/`⌘`+`⌥`+`K` shortcuts in Rider IDE to move to the commit window and commit/push.

- `xm` - extract method  
- `xp` - extract parameter  
- `xv` - extract variable  
- `xf` - extract field  
- `xc` - extract constant  
- `xC` - extract class  
- `iv` - inline variable  
- `im` - inline method  
- `ip` - inline parameter  
- `rm` - rename method  
- `rv` - rename variable  
- `rp` - rename parameter  
- `rf` - rename field  
- `mm` - move method  
- `fmt` - format  
- `rd` - remove duplication  
- `tda` - Tell Don’t Ask

_**Every change made should be deployable.**_  
If anyone in the group is feeling anxious about the risk of the change (they feel a change is too risky), we revert back to safety and do it in smaller, safer steps. Especially important in code that is not covered with tests or that we want to tweak enough to be able to test.


### Most Used Shortcuts

- Run all tests from the solution - `Command` + `;` + `L`  
- Run all tests with coverage from the solution - `Command` + `;` + `K`  
- Run last test session - `Command` + `;` + `Y`  
- Introduce a variable - `Command` + `Option` + `V`  
- Extract method - `Command` + `Option` + `M`  
- Introduce field (convert a local variable to a class field) - `Command` + `Option` + `F`  
- Introduce constant - `Command` + `Option` + `C`  
- Change method signature - `Command` + `F6`  
- Move static method - `F6`  
- Inline variable/method - `Command` + `Option` + `N`  
- Introduce parameter - `Command` + `Option` + `P`  
- Magic shortcut! Move a static method to a class of one of the parameter's and make it an instance method (also called Make Method Non-Static) - `Command` + `Option` + `I`  
- Expand selection - `Option` + `Up`  
- Shrink selection - `Option` + `Down`  
- Discard not committed changes - `Command` + `Option` + `Z`  
- Format code - `Command` + `Option` + `L`  
- Commit - `Command` + `K`  
- Push - `Command` + `Shift` + `K`  
- Rename method - `Shift` + `F6`  
- Go to method definition/find usages - `Command` + `B`  
- Move line up/down - `Command` + `Shift` + `Up`/`Down`  
