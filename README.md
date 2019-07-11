# Award weighted criteria extension for EU data

> OCDS extension to describe criteria as expressed in eForms (BG-707) and compatible with TED

This extension aims primarily at supporting criteria data formatted according to eForms data structure, but it also aims at enabling the OCDS publication of TED v2.0.9 data.

## Guidance for TED mapping

If only `AC_QUALITY` is set,  set `tender.awardCriteria` to "qualityOnly".

If only `AC_COST` is set, set `tender.awardCriteria` to "costOnly".

If only `AC_PRICE` is set, set `tender.awardCriteria` to "priceOnly".

If a mix of `AC_QUALITY`, `AC_COST` and `AC_PRICE` is set, set `tender.awardCriteria` to "ratedCriteria".

Add an `AwardWeightedCriteria` object to the `tender.awardWeightedCriteriaPerLot` array.

Set the `AwardWeightedCriteria` object as follow:

**AC_QUALITY**

Add an `AwardWeightedCriterion` object to the `awardWeightedCriteria` array.

Map `AC_CRITERION` to `criterionName`.

Map `AC_WEIGHTING` to `criterionDescription`.

Set `criterionType` to "quality".

**AC_COST**

Add an `AwardWeightedCriterion` object to the `awardWeightedCriteria` array.

Map `AC_CRITERION` to `criterionName`.

Map `AC_WEIGHTING` to `criterionDescription`.

Set `criterionType` to "cost".

**AC_PRICE**

Add an `AwardWeightedCriterion` object to the `awardWeightedCriteria` array.

Map `AC_CRITERION` to `criterionName`.

Map `AC_WEIGHTING` to `criterionDescription`.

Set `criterionType` to "price".

**AC_PROCUREMENT_DOC**

Discard.
