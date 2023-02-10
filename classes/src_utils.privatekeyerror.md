[dijets](../README.md) › [src/utils](../modules/src_utils.md) › [PrivateKeyError](src_utils.privatekeyerror.md)

# Class: PrivateKeyError

## Hierarchy

  ↳ [DijetsError](src_utils.dijetserror.md)

  ↳ **PrivateKeyError**

## Index

### Constructors

* [constructor](src_utils.privatekeyerror.md#constructor)

### Properties

* [errorCode](src_utils.privatekeyerror.md#errorcode)
* [message](src_utils.privatekeyerror.md#message)
* [name](src_utils.privatekeyerror.md#name)
* [stack](src_utils.privatekeyerror.md#optional-stack)

### Methods

* [getCode](src_utils.privatekeyerror.md#getcode)

## Constructors

###  constructor

\+ **new PrivateKeyError**(`m`: string): *[PrivateKeyError](src_utils.privatekeyerror.md)*

*Overrides [DijetsError](src_utils.dijetserror.md).[constructor](src_utils.dijetserror.md#constructor)*

*Defined in [src/utils/errors.ts:284](https://github.com/Dijets-Inc/dijetsjs/blob/ca67b81/src/utils/errors.ts#L284)*

**Parameters:**

Name | Type |
------ | ------ |
`m` | string |

**Returns:** *[PrivateKeyError](src_utils.privatekeyerror.md)*

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
