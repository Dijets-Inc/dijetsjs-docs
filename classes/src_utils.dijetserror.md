[dijets](../README.md) › [src/utils](../modules/src_utils.md) › [DijetsError](src_utils.dijetserror.md)

# Class: DijetsError

## Hierarchy

* [Error](src_utils.dijetserror.md#static-error)

  ↳ **DijetsError**

  ↳ [AddressError](src_utils.addresserror.md)

  ↳ [GooseEggCheckError](src_utils.gooseeggcheckerror.md)

  ↳ [ChainIdError](src_utils.chainiderror.md)

  ↳ [NoAtomicUTXOsError](src_utils.noatomicutxoserror.md)

  ↳ [SymbolError](src_utils.symbolerror.md)

  ↳ [NameError](src_utils.nameerror.md)

  ↳ [TransactionError](src_utils.transactionerror.md)

  ↳ [CodecIdError](src_utils.codeciderror.md)

  ↳ [CredIdError](src_utils.crediderror.md)

  ↳ [TransferableOutputError](src_utils.transferableoutputerror.md)

  ↳ [TransferableInputError](src_utils.transferableinputerror.md)

  ↳ [InputIdError](src_utils.inputiderror.md)

  ↳ [OperationError](src_utils.operationerror.md)

  ↳ [InvalidOperationIdError](src_utils.invalidoperationiderror.md)

  ↳ [ChecksumError](src_utils.checksumerror.md)

  ↳ [OutputIdError](src_utils.outputiderror.md)

  ↳ [UTXOError](src_utils.utxoerror.md)

  ↳ [InsufficientFundsError](src_utils.insufficientfundserror.md)

  ↳ [ThresholdError](src_utils.thresholderror.md)

  ↳ [SECPMintOutputError](src_utils.secpmintoutputerror.md)

  ↳ [EVMInputError](src_utils.evminputerror.md)

  ↳ [EVMOutputError](src_utils.evmoutputerror.md)

  ↳ [FeeAssetError](src_utils.feeasseterror.md)

  ↳ [StakeError](src_utils.stakeerror.md)

  ↳ [TimeError](src_utils.timeerror.md)

  ↳ [DelegationFeeError](src_utils.delegationfeeerror.md)

  ↳ [SubnetOwnerError](src_utils.subnetownererror.md)

  ↳ [BufferSizeError](src_utils.buffersizeerror.md)

  ↳ [AddressIndexError](src_utils.addressindexerror.md)

  ↳ [PublicKeyError](src_utils.publickeyerror.md)

  ↳ [MergeRuleError](src_utils.mergeruleerror.md)

  ↳ [Base58Error](src_utils.base58error.md)

  ↳ [PrivateKeyError](src_utils.privatekeyerror.md)

  ↳ [NodeIdError](src_utils.nodeiderror.md)

  ↳ [HexError](src_utils.hexerror.md)

  ↳ [TypeIdError](src_utils.typeiderror.md)

  ↳ [TypeNameError](src_utils.typenameerror.md)

  ↳ [UnknownTypeError](src_utils.unknowntypeerror.md)

  ↳ [Bech32Error](src_utils.bech32error.md)

  ↳ [EVMFeeError](src_utils.evmfeeerror.md)

  ↳ [InvalidEntropy](src_utils.invalidentropy.md)

  ↳ [ProtocolError](src_utils.protocolerror.md)

  ↳ [SubnetIdError](src_utils.subnetiderror.md)

  ↳ [SubnetThresholdError](src_utils.subnetthresholderror.md)

  ↳ [SubnetAddressError](src_utils.subnetaddresserror.md)

## Index

### Constructors

* [constructor](src_utils.dijetserror.md#constructor)

### Properties

* [errorCode](src_utils.dijetserror.md#errorcode)
* [message](src_utils.dijetserror.md#message)
* [name](src_utils.dijetserror.md#name)
* [stack](src_utils.dijetserror.md#optional-stack)
* [Error](src_utils.dijetserror.md#static-error)

### Methods

* [getCode](src_utils.dijetserror.md#getcode)

## Constructors

###  constructor

\+ **new DijetsError**(`m`: string, `code`: string): *[DijetsError](src_utils.dijetserror.md)*

*Defined in [src/utils/errors.ts:48](https://github.com/Dijets-Inc/dijetsjs/blob/master/src/utils/errors.ts#L48)*

**Parameters:**

Name | Type |
------ | ------ |
`m` | string |
`code` | string |

**Returns:** *[DijetsError](src_utils.dijetserror.md)*

## Properties

###  errorCode

• **errorCode**: *string*

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

___

### `Static` Error

▪ **Error**: *ErrorConstructor*

Defined in node_modules/typescript/lib/lib.es5.d.ts:1039

## Methods

###  getCode

▸ **getCode**(): *string*

*Defined in [src/utils/errors.ts:55](https://github.com/Dijets-Inc/dijetsjs/blob/master/src/utils/errors.ts#L55)*

**Returns:** *string*
