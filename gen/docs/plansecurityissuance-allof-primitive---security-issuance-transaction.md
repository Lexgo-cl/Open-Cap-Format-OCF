# Primitive - Security Issuance Transaction Schema

```txt
Primitives.Transactions.Issuance.BaseIssuance.schema.json#/allOf/0
```

Abstract object describing fields common to all issuance objects

| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                                                              |
| :------------------ | :--------- | :------------- | :----------- | :---------------- | :-------------------- | :------------------ | :-------------------------------------------------------------------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [PlanSecurityIssuance.schema.json*](../../schema/objects/transactions/issuance/PlanSecurityIssuance.schema.json "open original schema") |

## 0 Type

`object` ([Primitive - Security Issuance Transaction](plansecurityissuance-allof-primitive---security-issuance-transaction.md))

all of

*   all of

    *   [Object - BaseObject](issuer-allof-object---baseobject.md "check type definition")

# 0 Properties

| Property                                            | Type     | Required | Nullable       | Defined by                                                                                                                                                                                                                   |
| :-------------------------------------------------- | :------- | :------- | :------------- | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [custom_id](#custom_id)                             | `string` | Required | cannot be null | [Primitive - Security Issuance Transaction](baseissuance-properties-custom_id.md "Primitives.Transactions.Issuance.BaseIssuance.schema.json#/properties/custom_id")                                                          |
| [stakeholder_id](#stakeholder_id)                   | `string` | Required | cannot be null | [Primitive - Security Issuance Transaction](baseissuance-properties-stakeholder_id.md "Primitives.Transactions.Issuance.BaseIssuance.schema.json#/properties/stakeholder_id")                                                |
| [board_approval_date](#board_approval_date)         | `string` | Required | cannot be null | [Primitive - Security Issuance Transaction](issuer-properties-type---datestring.md "Types.DateString.schema.json#/properties/board_approval_date")                                                                           |
| [consideration](#consideration)                     | `object` | Required | cannot be null | [Primitive - Security Issuance Transaction](plansecurityissuance-properties-type---money.md "Types.Money.schema.json#/properties/consideration")                                                                             |
| [security_law_exemptions](#security_law_exemptions) | `array`  | Required | cannot be null | [Primitive - Security Issuance Transaction](baseissuance-properties-convertible---typessecurityexemptionschemajson-array.md "Primitives.Transactions.Issuance.BaseIssuance.schema.json#/properties/security_law_exemptions") |

## custom_id

A custom ID for this convertible (e.g. CN-1.)

`custom_id`

*   is required

*   Type: `string`

*   cannot be null

*   defined in: [Primitive - Security Issuance Transaction](baseissuance-properties-custom_id.md "Primitives.Transactions.Issuance.BaseIssuance.schema.json#/properties/custom_id")

### custom_id Type

`string`

## stakeholder_id

Id of the stakeholder that holds legal title to this convertible.

`stakeholder_id`

*   is required

*   Type: `string`

*   cannot be null

*   defined in: [Primitive - Security Issuance Transaction](baseissuance-properties-stakeholder_id.md "Primitives.Transactions.Issuance.BaseIssuance.schema.json#/properties/stakeholder_id")

### stakeholder_id Type

`string`

## board_approval_date

Type representing an ISO-8601 date, e.g. 2022-01-28

`board_approval_date`

*   is required

*   Type: `string` ([Type - DateString](issuer-properties-type---datestring.md))

*   cannot be null

*   defined in: [Primitive - Security Issuance Transaction](issuer-properties-type---datestring.md "Types.DateString.schema.json#/properties/board_approval_date")

### board_approval_date Type

`string` ([Type - DateString](issuer-properties-type---datestring.md))

### board_approval_date Constraints

**date**: the string must be a date string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")

## consideration

Type representing a monetary value in a specified currency code

`consideration`

*   is required

*   Type: `object` ([Type - Money](plansecurityissuance-properties-type---money.md))

*   cannot be null

*   defined in: [Primitive - Security Issuance Transaction](plansecurityissuance-properties-type---money.md "Types.Money.schema.json#/properties/consideration")

### consideration Type

`object` ([Type - Money](plansecurityissuance-properties-type---money.md))

## security_law_exemptions

List of security law exemptions (and applicable jurisdictions) for this convertible

`security_law_exemptions`

*   is required

*   Type: `object[]` ([Type - SecurityExemption](baseissuance-properties-convertible---typessecurityexemptionschemajson-array-type---securityexemption.md))

*   cannot be null

*   defined in: [Primitive - Security Issuance Transaction](baseissuance-properties-convertible---typessecurityexemptionschemajson-array.md "Primitives.Transactions.Issuance.BaseIssuance.schema.json#/properties/security_law_exemptions")

### security_law_exemptions Type

`object[]` ([Type - SecurityExemption](baseissuance-properties-convertible---typessecurityexemptionschemajson-array-type---securityexemption.md))