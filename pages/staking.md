# Staking for Freelancers 

To ensure that they get quality work, requesters can require freelancers to put in a stake by using our staking smart contract. When staking this amount, Fs, the freelancer asserts that the work they have completed is done accurately and fairly. The amount staked should be enough to be “skin in the game”, but not too much that it substantively hurts freelancers who may just need to improve the quality of their work to an industry accepted level.  However, Fs should be large enough to disincentivize bad actors from gaming the system, as well as pay for verifiers and the gas used by the network.

## Staking for Requesters 

Requesters stake an amount, Rs, in escrow to disincentivize them from acting in bad faith by rejecting work that is up to industry accepted standards.  This amount is used to pay verifiers and the gas required by the network to complete the verification process.


## Staking for Verifiers 

In a process similar to code review in the software industry, vetted industry professionals called “verifiers” review and confirm the validity of the work that has been submitted by freelancers.  Requesters determine whether they require verifiers and how many verifications are needed before the work is accepted.  Relative to freelancers, verifiers stake a smaller amount, Vs, since they are reputable industry professionals chosen by the community and thus less likely to act in bad faith.  However, this stake still ensures that verifiers still are properly incentivized to be thorough and accurate in their verifications. Often, more than one verifier is requested and each verifier’s stake is governed by a smart contract. The verifiers reach consensus, and the verifier loses their stake if their review was overturned.  

If verifiers do not reach consensus on the work accuracy, a new set of verifiers are asked to verify the task. The new verifiers will be paid through the lost stake of the verifier who was wrong in their previous assessment.


## Case I: consensus that work is acceptable, and Requestor agrees

If two or more verifiers reach consensus and validate that the work meets industry standards, then the bounty reward, Fr, is released from escrow and paid out to the freelancer.  The requestor’s staked, Rs, is distributed among the verifiers and also covers the gas required in the verification process.

## Case II: consensus that work is not acceptable, and Freelancer agrees

If the verifiers reach consensus and say the work is inaccurate and the freelancer concedes, the freelancer has an opportunity to redo the work within a given timeframe.    If the freelancer successfully completes completes the task on the second try, he or she is penalized Vr, and their total reward is Fr − Vr. If the freelancer fails to redo the work, they lose their original stake of Fs to cover the verifiers and gas.  The bounty reward, Fr, is released from escrow and returned to the requestor.

## Case III: consensus that work is not acceptable, but Freelancer objects
If the verifiers reach consensus and say the work is inaccurate but the freelancer objects, the freelancer will have to put in additional stake Fs2 and a second set of verifiers will review the work.  If the work is deemed acceptable in this second round of review, the Fs2 is returned to the freelancer and the first set of verifiers will lose their stake. If the work is deemed unacceptable in this second round of review, the freelancer loses both sets of stake, Fs + Fs2, and the bounty reward Fr is returned back to the requestor.

## Case IV: consensus that work is acceptable, but Requestor objects

If the verifiers reach consensus and say the work is acceptable, but the requestor objects, the requestor will have to put in additional stake Rs2 and a second set of (more qualified) verifiers will review the work.  If the work is deemed acceptable again in this second round of review, the bounty reward Fr is released from escrow to the freelancer, and the requestor loses both sets of stake Rs + Rs2. If the work is deemed unacceptable in this second round of review, the first set of verifiers will lose their stake, and the bounty reward Fr is returned back to the requestor.
