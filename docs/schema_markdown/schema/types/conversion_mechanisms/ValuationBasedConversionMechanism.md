:house: [Documentation Home](../../../../README.md)

---

### Conversion Mechanism - Valuation-Based Conversion Mechanism

`https://raw.githubusercontent.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/main/schema/types/conversion_mechanisms/ValuationBasedConversionMechanism.schema.json`

_Sets forth inputs and conversion mechanism based on valuations_

**Data Type:** `OCF TYPE`

**Properties:**

| Property                        | Type                                                                                                                                                                                                                                                                                                 | Description                                                                                                                                                                                                                         | Required   |
| ------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------- |
| type                            | **Constant:** `VALUATION_BASED_CONVERSION`                                                                                                                                                                                                                                                           | Scalar Constant                                                                                                                                                                                                                     | `REQUIRED` |
| valuation_type                  | `Enum - Valuation-Based Formula Type`</br></br>_Description:_ Enumeration types of valuation inputs that go into a formula - e.g. use a specified value (`FIXED`), a cap (`VALUATION_CAP`) or actual valuation (`ACTUAL`).</br></br>**ONE OF:** </br>&bull; FIXED </br>&bull; ACTUAL </br>&bull; CAP | Enumeration types of valuation inputs that go into a formula - e.g. use a specified value (`FIXED`), a cap (`VALUATION_CAP`) or actual valuation (`ACTUAL`).                                                                        | `REQUIRED` |
| valuation_amount                | [schema/types/Monetary](../Monetary.md)                                                                                                                                                                                                                                                              | If there is a specified valuation figure to use, what is it? Look to `valuation_type` to understand whether this represents, a max valuation (`CAP`), actual valuation at time of exercise (`ACTUAL`) or fixed valuation (`FIXED`). | -          |
| capitalization_definition       | `STRING`                                                                                                                                                                                                                                                                                             | How is company capitalization defined for purposes of exercise calculations? If possible, include the legal language from the instrument.                                                                                           | -          |
| capitalization_definition_rules | [schema/types/CapitalizationDefinitionRules](../CapitalizationDefinitionRules.md)                                                                                                                                                                                                                    | The rules for which types of securities would be included in the capitalization definition.                                                                                                                                         | -          |

**Source Code:** [schema/types/conversion_mechanisms/ValuationBasedConversionMechanism](../../../../../schema/types/conversion_mechanisms/ValuationBasedConversionMechanism.schema.json)

Copyright © 2024 Open Cap Table Coalition.