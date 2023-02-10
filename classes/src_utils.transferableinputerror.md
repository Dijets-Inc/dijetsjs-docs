[dijets](../README.md) › [src/utils](../modules/src_utils.md) › [TransferableInputError](src_utils.transferableinputerror.md)

# Class: TransferableInputError

## Hierarchy

  ↳ [DijetsError](src_utils.dijetserror.md)

  ↳ **TransferableInputError**

## Index

### Constructors

* [constructor](src_utils.transferableinputerror.md#constructor)

### Properties

* [errorCode](src_utils.transferableinputerror.md#errorcode)
* [message](src_utils.transferableinputerror.md#message)
* [name](src_utils.transferableinputerror.md#name)
* [stack](src_utils.transferableinputerror.md#optional-stack)

### Methods

* [getCode](src_utils.transferableinputerror.md#getcode)

## Constructors

###  constructor

\+ **new TransferableInputError**(`m`: string): *[TransferableInputError](src_utils.transferableinputerror.md)*

*Overrides [DijetsError](src_utils.dijetserror.md).[constructor](src_utils.dijetserror.md#constructor)*

*Defined in [src/utils/errors.ts:130](https://github.com/Dijets-Inc/dijetsjs/blob/master/src/utils/errors.ts#L130)*

**Parameters:**

Name | Type |
------ | ------ |
`m` | string |

**Returns:** *[TransferableInputError](src_utils.transferableinputerror.md)*

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
