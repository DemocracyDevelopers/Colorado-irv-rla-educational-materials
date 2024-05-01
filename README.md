# Colorado-irv-rla-educational-materials
This repository contains educational materials for IRV Risk Limiting Audits using RAIRE. The materials are designed for Colorado IRV RLAs, but should be helpful for anyone considering IRV RLAs.

- The [Slides](https://github.com/DemocracyDevelopers/Colorado-irv-rla-educational-materials/blob/main/RaireGuide_SlideDeck.pdf) are a visual description of the main ideas.
- The [Guide to RAIRE - Part 1](https://github.com/DemocracyDevelopers/Colorado-irv-rla-educational-materials/blob/main/A_Guide_to_RAIRE_Part_1.pdf) is a more detailed guide intended for election officials, audit board members, and interested members of the public.
- The [Guide to RAIRE - Part 2](https://github.com/DemocracyDevelopers/Colorado-irv-rla-educational-materials/blob/main/A_Guide_to_RAIRE_Part_2.pdf) contains detailed technical descriptions of the important calculations. It is intended for developers.
- The [Design Plan - v 1.0](https://github.com/DemocracyDevelopers/Colorado-irv-rla-educational-materials/blob/main/DesignPlan_v1.1.pdf) describes our proposal for editing [colorado-rla](https://github.com/cdos-rla/colorado-rla) to incorporate RAIRE. It is intended for people particularly interested in the details of the Colorado project.

You can write, test and visualize RAIRE assertions using our [Online Assertion Explainer](https://democracydevelopers.github.io/raire-rs)
which automates the process of drawing the elimination trees and verifying that the announced winner won.

You can start with the default assertions (already there) or add your own.

You can download [examples from the Guide To RAIRE](https://github.com/DemocracyDevelopers/raire-rs/tree/main/WebContent/example_assertions). Click on the .json file you want, select the whole contents, and copy-paste it into the `input` field of the Assertion Explainer.  Alternatively, you can download the files onto your own device and then click `browse` to upload them to the explainer tool.

You can also write your own.

Click the `Explain` button to display the trees. 

If a tree has a large part that is not relevant to the display, it is summarised by a small triangle with a number in it indicating how many nodes it summarises.

There are two different display options.

**Compressed** The compressed form shows all the assertion implications at once, labelling each branch with the assertion that rules it out. 

This version is most useful if you are already familiar with assertions and are using the visualiser to validate RAIRE's output for an audit.

This is the default.

**Sequential** The sequential form shows the effects of each assertion, step by step. At each step, the green node is the winner candidate in the assertion, while the pink node is the loser. Paths turn grey, and are then removed, when the assertion rules them out.

This version is most useful if you are learning about assertions. You can get this version by checking `Show effect of each assertion sequentially.`

In either case, it is important to check that all paths on all trees for all non-winners are removed.
