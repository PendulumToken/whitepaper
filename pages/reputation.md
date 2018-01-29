# Reputation and Trust

## Reputation Score

* To build trust between potential buyers and sellers, every participant has a global reputation score linked to their account. This reputation score is displayed very prominently within Pendulum, so maintaining a high reputation score is encouraged.

* Once a transaction is complete between a buyer and seller, each participant can leave a review for the other. Non-participants are not allowed to write a review. Each review is composed of a star rating from 1 to 5 stars, with an optional field for comments and skill endorsements.

* The global reputation score is a decimal from 1.0 to 5.0, representing the average of all review scores weighted by the voting power of that reviewer.

## Skill Endorsements

* Skill endorsements is a way to signal confidence of a particular skill in a person. Endorsements are public for anyone to see.

* Upon successful completion of a transaction, buyers can endorse one or more skills of the seller. A buyer cannot endorse the same skill twice for the same seller. 

* Skill endorsement is an important factor that buyers look at when deciding whether to do transaction with a seller.

* High skill endorsement is one of the criteria in being a verifier of transactions involving that skill.

## Trust Graph

* Trust graph is a weighted directed graph representing the people you trust to do business again. For the initial phase, all edge weights are 1.0. In the future, we may change the weight to reflect degrees of trust between two parties.

* Trust edge can be formed from one user (truster) to another user (trusteee) upon successfully completing at least one transaction with each other. After which, one user can choose to declare the other user as "trusted". No acknowledgement is required from the trustee as this declaration of trust is unidirectional from truster to the trustee.

* Trust edge can be revoked at any time by the truster.

* Trust graph can be useful in several ways:
    * As a bookmark of people you would like to do business again.
    * As a signal to see who in your trust network also trust this person, acting as a indirect referral or trust score.
    * As a way to market the trustiness of the buyer or seller to the public.
  
* Open Question: Should the trust graph be public information to everybody or private to the user only or private between the trusted parties?