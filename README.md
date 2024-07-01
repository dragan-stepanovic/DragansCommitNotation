# Dragan's Commit Notation and Most Used Shortcuts (for IntelliJ IDEs)


### Commit notation
_Heuristic_: **Keep commit messages short to reduce the relative cost of committing compared to the size of a change**.  
The easier and faster it is to commit, the more often I'll do it, the smaller the changes I'll be making.  
In Lean terms, this commit notation reduces batch transaction cost which enables smaller batches and more frequent integration.    

Nice thing about refactorings (initially described in Martin Fowler's [Refactoring book](https://martinfowler.com/books/refactoring.html)) is that you most often need just two letters to represent them uniquely in a way that it's easy to remember them. That helps me with being able to make committing tiny changes so cheap (reducing transaction cost) that I can often commit multiple times per minute (smaller batches) without feeling that committing is slowing me down (higher flow efficiency) while minimizing cognitive load of not having to think about the changes I didn't yet commit (lower inventory).

<img width="865" alt="image" src="https://github.com/dragan-stepanovic/DragansCommitNotation/assets/332947/803fcc19-0121-49d9-82e6-42394659d8a0">

#### Rename
- `rm` - rename method  
- `rv` - rename variable  
- `rp` - rename parameter  
- `rf` - rename field
- `rc` - rename constant
- `rC` - rename class

#### Extract
- `xm` - extract method  
- `xv` - extract variable  
- `xp` - extract parameter  
- `xf` - extract field  
- `xc` - extract constant  
- `xC` - extract class  

#### Inline
- `im` - inline method  
- `iv` - inline variable  
- `ip` - inline parameter  
- `if` - inline field  

#### Move
- `mm` - move method  
- `tda` - Tell Don’t Ask

#### Misc
- `rd` - remove duplication  
- `fmt` - format  

_Heuristic_: _**Every change commited must be deployable to production. If a commit is not deployable, the change is most likely not sufficiently small. Find smaller step(s) instead.**_  
If anyone in the group is feeling anxious about the risk of a change (they feel a change is too risky), we revert back to safety and do it in smaller, safer steps. Anxiety about the step is useful feedback about the risk and size of the change. That is especially important in code that is not covered with tests or that we need to tweak enough to be able to get it under test (catch 22).


### Most Used Shortcuts

#### Refactorings  
- Rename method - `Shift` + `F6`
- Extract method - `Command` + `Option` + `M`
- Extract variable - `Command` + `Option` + `V`
- Extract field (convert a local variable to a class field) - `Command` + `Option` + `F`  
- Extract constant - `Command` + `Option` + `C`
- Extract parameter - `Command` + `Option` + `P`  
- Inline variable/method - `Command` + `Option` + `N`  

- Change method signature - `Command` + `F6`  
- Move static method - `F6`  
- Magic shortcut! Move a static method to a class of one of the parameter's and make it an instance method (also called Make Method Non-Static) - `Command` + `Option` + `I`  

- Format code - `Command` + `Option` + `L`  

#### Committing and Pushing  
- Open commit dialog - `Command` + `K`
- Commit (once in the commit dialog) - `Command` + `Enter`
- Push - `Command` + `Shift` + `K`
- Commit and push - `Command` + `Option` + `K`
- Move from commit dialog to code editor - `Esc`
- Discard uncommitted changes - `Command` + `Option` + `Z` (if you want to discard all changes you can then `Command` + `A` + `Space` to select all files and then `Option` + `R`)

#### Tests  
- Run all tests in solution - `Command` + `;` + `L`  
- Run last test session - `Command` + `;` + `Y`  
- Run all tests with coverage - `Command` + `;` + `K`  

#### Code Navigation and Selection  
- Go to method definition/find usages - `Command` + `B`
- Expand selection - `Option` + `Up`  
- Shrink selection - `Option` + `Down`  
- Move line/code block/method up/down - `Command` + `Shift` + `Up`/`Down`  
