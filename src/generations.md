In Rimworld's Biotech expansion, you can make cool custom genomes for your colonists. 
However, getting those genes to propogate correctly to future generations can be complicated.

This short guide contains everything you need to know to make multi-generational colonies with a persistent custom xenotype.

It covers the basics of pawn reproduction, gene inheritance, xenotype propogation, and inbreeding avoidance.

# Colonist Reproduction

There are two primary ways colonists can reproduce:

**Lovin'** between two fertile pawns with opposite sexes may result in pregnancy.
Pregnancy last 18 days.

**IVF** is a procedure that requires research. 
It involves removing a female colonist's ovum via a surgury and having a male colonist fertilize it.
Once fertilized, one of three things can be done with the embryo:
- It can be implanted back into the mother
- It can be implanted into a surrogate mother
- It can be placed in a Growth vat

## Growth vats

Embryos placed in a Growth vat take 9 days and adequate nutrition to produce a baby.

Any pawn below the age of 18 can be placed in a growth vat to age more quickly,
but growing a child in a vat prevents you from being able to choose their traits and passions.

# Gene Inheritance

Gene inheritance is somewhat complicated.

First, only germline genes can be inherited.
Germline genes are present in the following base xenotypes:
- Dirtmole
- Neanderthal
- Pigskin
- Impid
- Waster
- Yttakin

The rest of the base xenotypes only have xenogenes, which cannot be passed on to children.

Custom xenotypes can be made inheritable by checking "Genes are heritable" at the bottom of the xenotype editor.
For the rest of this section "genes" will refer only to germline genes.

When combining two pawns' genes, there are two modes.
Which one is used depends on how similar their genomes are.

**If any genes other than baseline hair and skin color are different**, then each gene of each parent has a roughly 50% chance of being passed on to the child genome. The resulting child's xenotype will be baseliner.

**If both genomes have all the same genes other than baseline hair and skin color**, then the resulting combined genome will have all the same non-color genes as the parents, and the color genes will be combined according to the first mode. If the parent xenotypes have different names, then the name of the mother's xenotype will be used.

# Inbreeding

Pawns will never (and cannot be persuaded) to romance anyone with whom they have a blood relation.

While IVF can still be used on blood-related pawns, it can cause the resulting child to have *Inbred* as a germline gene.
*Inbred* forces the *Slow Learner* trait and adds Fertility x50% and Immunity gain speed x85%.

Because it is a germline gene that can be passed on the subsequent children, it should go without saying that inbreeding is to be avoided.

The chance of inbreeding occuring is dependent on how close the blood relation is:

| Relationship                  | *Inbred* chance |
| ----------------------------- | --------------- |
| Parent/Child                  | 80%             |
| Sibling                       | 80%             |
| Grand parent/child            | 40%             |
| Aunt/Uncle/Niece/Nephew       | 40%             |
| Cousin                        | 20%             |
| Great grand parent/child      | 10%             |
| Grand aunt/uncle/niece/nephew | 10%             |
| Cousin once removed           | 10%             |
| Second cousin                 | 10%             |

I have not tested the chances for more distant pawn relations, so I am unsure if they are ever considered distant enough for romance.
Going through the steps to create 2 pawns that were second cousins for testing was an ordeal in itself, even with dev mode.

# Multi-generational colonies

A multi-generation colony is easy when you don't care about xenotypes. Simply allow starting pawns to reproduce with joining pawns.

If you want to preserve one of the six base germline xenotypes listed above, then simply promote reproduction between starting pawns and joining pawns *of that xenotype*. i.e. If you want to have multiple generations of Impids, then promote Impid reproduction.

However, if the xenotype you want to preserve is a custom one, then things get more complicated.
The only pawns you will ever see with a custom inheritable xenotype are your starting pawns.
This means that you will have to closely monitor relationships and carefuly plan IVF rounds in order to keep it going without losing genes.

The Lost Tribe start has the most starting pawns of any default scenario, and even with the 5 it gives you, eventually encountering a 20% chance of the *Inbred* gene is unnavoidable.

I recommend using a custom scenario.
The number of required starting pawns increases exponentially with the desired maximum genetic difference of future generations.
Make sure that there are an equal number of starting men and women too!

| Maximum genetic difference | *Inbred* chance | Starting pawns required |
| -------------------------- | --------------- | ----------------------- |
| Siblings                   | 80%             | 2                       |
| Cousins                    | 20%             | 4                       |
| Second cousins             | 10%             | 8                       |
| Third cousins              | ?               | 16                      |

If you want to have a multi-generation colony in a timely manner, I would also recommend increasing child and adult aging rates in the storyteller settings.