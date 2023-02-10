[dijets](../README.md) › [src/utils](../modules/src_utils.md) › [UTXOError](src_utils.utxoerror.md)

# Class: UTXOError

## Hierarchy

  ↳ [DijetsError](src_utils.dijetserror.md)

  ↳ **UTXOError**

## Index

### Constructors

* [constructor](src_utils.utxoerror.md#constructor)

### Properties

* [errorCode](src_utils.utxoerror.md#errorcode)
* [message](src_utils.utxoerror.md#message)
* [name](src_utils.utxoerror.md#name)
* [stack](src_utils.utxoerror.md#optional-stack)

### Methods

* [getCode](src_utils.utxoerror.md#getcode)

## Constructors

###  constructor

\+ **new UTXOError**(`m`: string): *[UTXOError](src_utils.utxoerror.md)*

*Overrides [DijetsError](src_utils.dijetserror.md).[constructor](src_utils.dijetserror.md#constructor)*

*Defined in [src/utils/errors.ts:172](https://github.com/Dijets-Inc/dijetsjs/blob/ca67b81/src/utils/errors.ts#L172)*

**Parameters:**

Name | Type |
------ | ------ |
`m` | string |

**Returns:** *[UTXOError](src_utils.utxoerror.md)*

## Properties

###  errorCode

• **errorCode**: *string*

*Inherited from [DijetsError](src_utils.dijetserror.md).[errorCode](src_utils.dijetserror.md#errorcode)*

*Defined in [src/utils/errors.ts:48](https://github.com/Dijets-Inc/dijetsjs/blob/ca67b81/src/utils/errors.ts#L48)*

___

###  message

• **message**: *string*

*Inherited from [DijetsError](src_utils.dijetserror.md).[message](src_utils.dijetserror.md#message)*

Defined in node_modules/typescript/lib/lib.es5.d.ts:1029

___

###  name

• **name**: *string*

*Inherited from [DijetsError](src_utils.dijetserror.md).[name](src_utils.dijetserror.md#name)*

Defined in node_modules/typescript/lib/lib.es5.d.ts:1028

___

### `Optional` stack

• **stack**? : *string*

*Inherited from [DijetsError](src_utils.dijetserror.md).[stack](src_utils.dijetserror.md#optional-stack)*

Defined in node_modules/typescript/lib/lib.es5.d.ts:1030

## Methods

###  getCode

▸ **getCode**(): *string*

*Inherited from [DijetsError](src_utils.dijetserror.md).[getCode](src_utils.dijetserror.md#getcode)*

*Defined in [src/utils/errors.ts:55](https://github.com/Dijets-Inc/dijetsjs/blob/ca67b81/src/utils/errors.ts#L55)*

**Returns:** *string*
