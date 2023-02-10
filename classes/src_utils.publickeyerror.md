[dijets](../README.md) › [src/utils](../modules/src_utils.md) › [PublicKeyError](src_utils.publickeyerror.md)

# Class: PublicKeyError

## Hierarchy

  ↳ [DijetsError](src_utils.dijetserror.md)

  ↳ **PublicKeyError**

## Index

### Constructors

* [constructor](src_utils.publickeyerror.md#constructor)

### Properties

* [errorCode](src_utils.publickeyerror.md#errorcode)
* [message](src_utils.publickeyerror.md#message)
* [name](src_utils.publickeyerror.md#name)
* [stack](src_utils.publickeyerror.md#optional-stack)

### Methods

* [getCode](src_utils.publickeyerror.md#getcode)

## Constructors

###  constructor

\+ **new PublicKeyError**(`m`: string): *[PublicKeyError](src_utils.publickeyerror.md)*

*Overrides [DijetsError](src_utils.dijetserror.md).[constructor](src_utils.dijetserror.md#constructor)*

*Defined in [src/utils/errors.ts:263](https://github.com/Dijets-Inc/dijetsjs/blob/master/src/utils/errors.ts#L263)*

**Parameters:**

Name | Type |
------ | ------ |
`m` | string |

**Returns:** *[PublicKeyError](src_utils.publickeyerror.md)*

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
