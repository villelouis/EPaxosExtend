EPaxos with Quorum update
--
This spec is updated version of [epaxos](https://github.com/efficient/epaxos) \
Description of Epaxos and useful information can be found here [egalitarian-paxos](https://github.com/tlaplus/Examples/tree/master/specifications/egalitarian-paxos)  \
This spec expose epaxos spec with addition of a replica
#
Model
--
### Model Overview
#### Constants:
```
MaxBallot <- 2
Commands <- <symmetrical>  {c1,c2}
```
Deadlock uncheck 
#### Invariants:
`TypeOK`
