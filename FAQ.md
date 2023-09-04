# Frequently Asked Questions about IRV RLAs with RAIRE

## Question 1: Can I be confident in the results audited by RAIRE?
Answer: Yes. IRV RLAs with RAIRE satisfy a risk limit, just like any other Risk Limiting Audit. This limits the probability of mistakenly accepting a wrong outcome.

## Question 2: Will these audits require more ballot samples than plurality RLAs?
Answer: No. The number of ballot samples depends on the contest margin and the number of errors found during the audit. 
IRV RLAs with RAIRE require approximately the same sample size as plurality audits with the same margin and error rate.

Sometimes it is hard to understand the true margin of an IRV contest---if the IRV contest has a close comparison somewhere in the elimination 
sequence that makes a difference to the outcome, then RAIRE will identify that comparison and may require a lot of samples to audit it. This is
equivalent to a plurality contest with the same small margin.

## Question 3: How does an RLA change when using ranked choice voting?
Answer: The process does not change. The dice rolling, random selection of ballots, and entry of sampled ballots into CORLA by the audit board will all be exactly the same. The underlying math for testing the outcome changes. 

See the [Guide to RAIRE](https://github.com/DemocracyDevelopers/Colorado-irv-rla-educational-materials/blob/main/A_Guide_to_RAIRE_Part_1.pdf) for more details.

## Question 4: What assertions are made using RAIRE?
Answer: There are two main types of assertions. Never Eliminated Before (NEB) and Not Eliminated Next (NEN). NEN assertions compare two candidates in a particular context, where a specific set of candidates remains standing, and assert that the winner has a higher tally than the loser at that point. An NEB assertion says that, no matter what happens, one candidate always has a higher tally than another. 

You can examine some example assertions, and write and test your own, with our [online assertion explainer](https://democracydevelopers.github.io/raire-rs/WebContent/explain_assertions.html).

## Question 5: What are overstatements and understatements in RAIRE?
Answer: Overstatements and understatements relate to each assertion. An overstatement is an error in the cast vote record that inflates the assertion's margin. That is, it makes the winner seem to have won by more than they really did. 
An understatement is the opposite. Some examples are given in slides 33 and 35 of the [Slide Deck](https://github.com/DemocracyDevelopers/Colorado-irv-rla-educational-materials/blob/main/RaireGuide_SlideDeck.pdf).

## Question 6: Will the code be open source?
Answer: Yes. You can watch the development in our [Github repositories here](https://github.com/DemocracyDevelopers/). The final product will 
eventually be incorporated into [The Colorado RLA repositories](https://github.com/cdos-rla). 
