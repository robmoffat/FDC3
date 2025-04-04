---
title: cdm.PriceQuantity
sidebar_label: cdm.PriceQuantity

---

# cdm.PriceQuantity

[@experimental](/docs/fdc3-compliance#experimental-features) example of bringing in the CDM PriceQuantity object into FDC3

## Schema

[/schemas/next/context/priceQuantity.schema.json](/schemas/next/context/priceQuantity.schema.json) ([github](https://github.com/finos/FDC3/tree/main/packages/fdc3-context/schemas/context/priceQuantity.schema.json))

## Type

`cdm.observable.asset.PriceQuantity`

## Properties

<details>
  <summary><code>data</code> <strong>(required)</strong></summary>

**type**: `object`

</details>

## Example

```json
{
  "type": "cdm.observable.asset.PriceQuantity",
  "data": {
    "price": [
      {
        "value": {
          "priceExpression": "PerUnitOfAmount",
          "priceType": "Clean",
          "price": [
            {
              "value": 99.75
            }
          ],
          "perUnitOfAmount": {
            "currency": "USD"
          }
        }
      }
    ],
    "quantity": [
      {
        "value": {
          "schedule": [
            {
              "value": 1000000
            }
          ],
          "unitOfMeasure": "USD"
        }
      }
    ],
    "observable": {
      "value": {
        "productIdentifier": [
          {
            "identifier": "US1234567890",
            "source": "CUSIP"
          }
        ]
      }
    },
    "effectiveDate": {
      "adjustableDate": {
        "unadjustedDate": "2025-04-01",
        "dateAdjustments": {
          "businessDayConvention": "FOLLOWING",
          "businessCenters": {
            "businessCenter": [
              "USNY"
            ]
          }
        }
      }
    }
  }
}
```

