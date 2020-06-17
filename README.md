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
Replicas <- <symmetrical>  {r1,r2,r3}
Commands <- <symmetrical>  {c1,c2}
FastQuorums(X) <- IF X=r1 THEN {{r1,r3}}
                  ELSE IF X=r2 THEN {{r2,r3}}
                  ELSE {{r3,r2}}
SlowQuorums(X) <- IF X=r1 THEN {{r1,r3}}
                  ELSE IF X=r2 THEN {{r2,r3}}
                  ELSE {{r3,r2}}
```
Deadlock uncheck 
#### Invariants:
`TypeOK`
