# Award criteria breakdown

Adds an award criteria breakdown array to the tender object, to break down award criteria by price, cost and quality.

## Legal context

In the European Union, this extension's fields correspond to [eForms BG-707 (Award Criteria)](https://github.com/eForms/eForms). See [OCDS for the European Union](http://standard.open-contracting.org/profiles/eu/master/en/) for the correspondences to Tenders Electronic Daily (TED).

[Directive 2014/24/EU](https://eur-lex.europa.eu/eli/dir/2014/24/oj) [Article 67](https://eur-lex.europa.eu/eli/dir/2014/24/oj#d1e5950-65-1)(5) describes weightings and orders of importance.

## Example

```json
{
  "tender": {
    "awardCriteriaBreakdown": [
      {
        "relatedLots": [
          "1",
          "2"
        ],
        "awardCriteria": [
          {
            "type": "quality",
            "name": "Service quality",
            "numbers": [
              {
                "number": 50,
                "weight": "percentageExact"
              }
            ]
          },
          {
            "type": "price",
            "name": "Price",
            "numbers": [
              {
                "number": 50,
                "weight": "percentageExact"
              }
            ]
          }
        ]
      }
    ]
  }
}
```

## Issues

Report issues for this extension in the [ocds-extensions repository](https://github.com/open-contracting/ocds-extensions/issues), putting the extension's name in the issue's title.

## Changelog

This model was discussed in <https://github.com/eForms/eForms/issues/119>, <https://github.com/eprocurementontology/eprocurementontology/issues/157> and <https://github.com/eprocurementontology/eprocurementontology/issues/203>.
