[dijets](../README.md) › [src/utils](../modules/src_utils.md) › [SymbolError](src_utils.symbolerror.md)

# Class: SymbolError

## Hierarchy

  ↳ [DijetsError](src_utils.dijetserror.md)

  ↳ **SymbolError**

## Index

### Constructors

* [constructor](src_utils.symbolerror.md#constructor)

### Properties

* [errorCode](src_utils.symbolerror.md#errorcode)
* [message](src_utils.symbolerror.md#message)
* [name](src_utils.symbolerror.md#name)
* [stack](src_utils.symbolerror.md#optional-stack)

### Methods

* [getCode](src_utils.symbolerror.md#getcode)

## Constructors

###  constructor

\+ **new SymbolError**(`m`: string): *[SymbolError](src_utils.symbolerror.md)*

*Overrides [DijetsError](src_utils.dijetserror.md).[constructor](src_utils.dijetserror.md#constructor)*

*Defined in [src/utils/errors.ts:88](https://github.com/Dijets-Inc/dijetsjs/blob/master/src/utils/errors.ts#L88)*

**Parameters:**

Name | Type |
------ | ------ |
`m` | string |

**Returns:** *[SymbolError](src_utils.symbolerror.md)*

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
