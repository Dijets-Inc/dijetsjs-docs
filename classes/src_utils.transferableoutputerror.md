[dijets](../README.md) › [src/utils](../modules/src_utils.md) › [TransferableOutputError](src_utils.transferableoutputerror.md)

# Class: TransferableOutputError

## Hierarchy

  ↳ [DijetsError](src_utils.dijetserror.md)

  ↳ **TransferableOutputError**

## Index

### Constructors

* [constructor](src_utils.transferableoutputerror.md#constructor)

### Properties

* [errorCode](src_utils.transferableoutputerror.md#errorcode)
* [message](src_utils.transferableoutputerror.md#message)
* [name](src_utils.transferableoutputerror.md#name)
* [stack](src_utils.transferableoutputerror.md#optional-stack)

### Methods

* [getCode](src_utils.transferableoutputerror.md#getcode)

## Constructors

###  constructor

\+ **new TransferableOutputError**(`m`: string): *[TransferableOutputError](src_utils.transferableoutputerror.md)*

*Overrides [DijetsError](src_utils.dijetserror.md).[constructor](src_utils.dijetserror.md#constructor)*

*Defined in [src/utils/errors.ts:123](https://github.com/Dijets-Inc/dijetsjs/blob/master/src/utils/errors.ts#L123)*

**Parameters:**

Name | Type |
------ | ------ |
`m` | string |

**Returns:** *[TransferableOutputError](src_utils.transferableoutputerror.md)*

## Properties

###  errorCode

• **errorCode**: *string*

*Inherited from [DijetsError](src_utils.dijetserror.md).[errorCode](src_utils.dijetserror.md#errorcode)*

*Defined in [src/utils/errors.ts:48](https://github.com/Dijets-Inc/dijetsjs/blob/master/src/utils/errors.ts#L48)*

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

*Defined in [src/utils/errors.ts:55](https://github.com/Dijets-Inc/dijetsjs/blob/master/src/utils/errors.ts#L55)*

**Returns:** *string*
