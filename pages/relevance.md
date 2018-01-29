# Relevance

* Discovery and relevance is key to matching buyers and sellers.


## Searching

* For performance and scalability reasons, search is performed off-chain on cloud servers via REST API.

* All user profiles are cached for performance, and indexed for fast searching. For the initial phase, we will use the good old-fashion PostgreSQL query.


## Relevance Scoring

* Relevance can be calculated per user given the following matching criteria:
    - Keywords
    - Skills
    - Interests
    - Availability
   
* Relevance is scored as a positive floating number from 0.0 (least) to 1.0 (most) and is calculated based on following factors:
    - Match score of keywords
    - Match score of skills weighted by endorsements
    - Match score of intersts
    - Match score of availability
    - Reputation of seller
    - Trusted by buyer

    - Relevance Score = normalizedScore((KeywordWeight * KeywordMatchScore) + (SkillWeight * SkillMatchScore) + (InterestWeight * InterestMatchScore) + (AvailabilityWeight * AvailabilityMatchScore) + (ReputationWeight * ReputationScore) + (TrustWeight * TrustScore))