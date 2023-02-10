[dijets](../README.md) › [Dijets](../modules/dijets.md) › [Dijets](dijets.dijets-1.md)

# Class: Dijets

DijetsJS is middleware for interacting with Dijets node RPC APIs.

Example usage:
```js
const dijets: Dijets = new Dijets("127.0.0.1", 9650, "https")
```

## Hierarchy

* [DijetsCore](dijetscore.dijetscore-1.md)

  ↳ **Dijets**

## Index

### Constructors

* [constructor](dijets.dijets-1.md#constructor)

### Properties

* [apis](dijets.dijets-1.md#protected-apis)
* [auth](dijets.dijets-1.md#protected-auth)
* [baseEndpoint](dijets.dijets-1.md#protected-baseendpoint)
* [headers](dijets.dijets-1.md#protected-headers)
* [host](dijets.dijets-1.md#protected-host)
* [hrp](dijets.dijets-1.md#protected-hrp)
* [ip](dijets.dijets-1.md#protected-ip)
* [networkID](dijets.dijets-1.md#protected-networkid)
* [port](dijets.dijets-1.md#protected-port)
* [protocol](dijets.dijets-1.md#protected-protocol)
* [requestConfig](dijets.dijets-1.md#protected-requestconfig)
* [url](dijets.dijets-1.md#protected-url)

### Methods

* [Admin](dijets.dijets-1.md#admin)
* [Auth](dijets.dijets-1.md#auth)
* [CChain](dijets.dijets-1.md#cchain)
* [Health](dijets.dijets-1.md#health)
* [Index](dijets.dijets-1.md#index)
* [Info](dijets.dijets-1.md#info)
* [Metrics](dijets.dijets-1.md#metrics)
* [NodeKeys](dijets.dijets-1.md#nodekeys)
* [PChain](dijets.dijets-1.md#pchain)
* [XChain](dijets.dijets-1.md#xchain)
* [_setHeaders](dijets.dijets-1.md#protected-_setheaders)
* [addAPI](dijets.dijets-1.md#addapi)
* [api](dijets.dijets-1.md#api)
* [delete](dijets.dijets-1.md#delete)
* [get](dijets.dijets-1.md#get)
* [getBaseEndpoint](dijets.dijets-1.md#getbaseendpoint)
* [getHRP](dijets.dijets-1.md#gethrp)
* [getHeaders](dijets.dijets-1.md#getheaders)
* [getHost](dijets.dijets-1.md#gethost)
* [getIP](dijets.dijets-1.md#getip)
* [getNetworkID](dijets.dijets-1.md#getnetworkid)
* [getPort](dijets.dijets-1.md#getport)
* [getProtocol](dijets.dijets-1.md#getprotocol)
* [getRequestConfig](dijets.dijets-1.md#getrequestconfig)
* [getURL](dijets.dijets-1.md#geturl)
* [patch](dijets.dijets-1.md#patch)
* [post](dijets.dijets-1.md#post)
* [put](dijets.dijets-1.md#put)
* [removeAllHeaders](dijets.dijets-1.md#removeallheaders)
* [removeAllRequestConfigs](dijets.dijets-1.md#removeallrequestconfigs)
* [removeHeader](dijets.dijets-1.md#removeheader)
* [removeRequestConfig](dijets.dijets-1.md#removerequestconfig)
* [setAddress](dijets.dijets-1.md#setaddress)
* [setAuthToken](dijets.dijets-1.md#setauthtoken)
* [setHRP](dijets.dijets-1.md#sethrp)
* [setHeader](dijets.dijets-1.md#setheader)
* [setNetworkID](dijets.dijets-1.md#setnetworkid)
* [setRequestConfig](dijets.dijets-1.md#setrequestconfig)

## Constructors

###  constructor

\+ **new Dijets**(`host?`: string, `port?`: number, `protocol`: string, `networkID`: number, `XChainID`: string, `CChainID`: string, `hrp`: string, `skipinit`: boolean): *[Dijets](dijets.dijets-1.md)*

*Overrides [DijetsCore](dijetscore.dijetscore-1.md).[constructor](dijetscore.dijetscore-1.md#constructor)*

*Defined in [src/index.ts:88](https://github.com/Dijets-Inc/dijetsjs/blob/ca67b81/src/index.ts#L88)*

Creates a new Dijets instance. Sets the address and port of the main Dijets Client.

**Parameters:**

Name | Type | Default | Description |
------ | ------ | ------ | ------ |
`host?` | string | - | The hostname to resolve to reach the Dijets Client RPC APIs |
`port?` | number | - | The port to resolve to reach the Dijets Client RPC APIs |
`protocol` | string | "http" | The protocol string to use before a "://" in a request, ex: "http", "https", "git", "ws", etc. Defaults to http |
`networkID` | number | DefaultNetworkID | Sets the NetworkID of the class. Default [DefaultNetworkID](../modules/utils_constants.md#const-defaultnetworkid) |
`XChainID` | string | undefined | Sets the blockchainID for the AVM. Will try to auto-detect, otherwise default "2eNy1mUFdmaxXNj1eQHUe7Np4gju9sJsEtWQ4MX3ToiNKuADed" |
`CChainID` | string | undefined | Sets the blockchainID for the EVM. Will try to auto-detect, otherwise default "2CA6j5zYzasynPsFeNoqWkmTCt3VScMvXUZHbfDJ8k3oGzAPtU" |
`hrp` | string | undefined | The human-readable part of the bech32 addresses |
`skipinit` | boolean | false | Skips creating the APIs. Defaults to false  |

**Returns:** *[Dijets](dijets.dijets-1.md)*

## Properties

### `Protected` apis

• **apis**: *object*

*Inherited from [DijetsCore](dijetscore.dijetscore-1.md).[apis](dijetscore.dijetscore-1.md#protected-apis)*

*Defined in [src/dijets.ts:38](https://github.com/Dijets-Inc/dijetsjs/blob/ca67b81/src/dijets.ts#L38)*

#### Type declaration:

* \[ **k**: *string*\]: [APIBase](common_apibase.apibase.md)

___

### `Protected` auth

• **auth**: *string* = undefined

*Inherited from [DijetsCore](dijetscore.dijetscore-1.md).[auth](dijetscore.dijetscore-1.md#protected-auth)*

*Defined in [src/dijets.ts:35](https://github.com/Dijets-Inc/dijetsjs/blob/ca67b81/src/dijets.ts#L35)*

___

### `Protected` baseEndpoint

• **baseEndpoint**: *string*

*Inherited from [DijetsCore](dijetscore.dijetscore-1.md).[baseEndpoint](dijetscore.dijetscore-1.md#protected-baseendpoint)*

*Defined in [src/dijets.ts:33](https://github.com/Dijets-Inc/dijetsjs/blob/ca67b81/src/dijets.ts#L33)*

___

### `Protected` headers

• **headers**: *object*

*Inherited from [DijetsCore](dijetscore.dijetscore-1.md).[headers](dijetscore.dijetscore-1.md#protected-headers)*

*Defined in [src/dijets.ts:36](https://github.com/Dijets-Inc/dijetsjs/blob/ca67b81/src/dijets.ts#L36)*

#### Type declaration:

* \[ **k**: *string*\]: string

___

### `Protected` host

• **host**: *string*

*Inherited from [DijetsCore](dijetscore.dijetscore-1.md).[host](dijetscore.dijetscore-1.md#protected-host)*

*Defined in [src/dijets.ts:31](https://github.com/Dijets-Inc/dijetsjs/blob/ca67b81/src/dijets.ts#L31)*

___

### `Protected` hrp

• **hrp**: *string* = ""

*Inherited from [DijetsCore](dijetscore.dijetscore-1.md).[hrp](dijetscore.dijetscore-1.md#protected-hrp)*

*Defined in [src/dijets.ts:28](https://github.com/Dijets-Inc/dijetsjs/blob/ca67b81/src/dijets.ts#L28)*

___

### `Protected` ip

• **ip**: *string*

*Inherited from [DijetsCore](dijetscore.dijetscore-1.md).[ip](dijetscore.dijetscore-1.md#protected-ip)*

*Defined in [src/dijets.ts:30](https://github.com/Dijets-Inc/dijetsjs/blob/ca67b81/src/dijets.ts#L30)*

___

### `Protected` networkID

• **networkID**: *number* = 0

*Inherited from [DijetsCore](dijetscore.dijetscore-1.md).[networkID](dijetscore.dijetscore-1.md#protected-networkid)*

*Defined in [src/dijets.ts:27](https://github.com/Dijets-Inc/dijetsjs/blob/ca67b81/src/dijets.ts#L27)*

___

### `Protected` port

• **port**: *number*

*Inherited from [DijetsCore](dijetscore.dijetscore-1.md).[port](dijetscore.dijetscore-1.md#protected-port)*

*Defined in [src/dijets.ts:32](https://github.com/Dijets-Inc/dijetsjs/blob/ca67b81/src/dijets.ts#L32)*

___

### `Protected` protocol

• **protocol**: *string*

*Inherited from [DijetsCore](dijetscore.dijetscore-1.md).[protocol](dijetscore.dijetscore-1.md#protected-protocol)*

*Defined in [src/dijets.ts:29](https://github.com/Dijets-Inc/dijetsjs/blob/ca67b81/src/dijets.ts#L29)*

___

### `Protected` requestConfig

• **requestConfig**: *AxiosRequestConfig*

*Inherited from [DijetsCore](dijetscore.dijetscore-1.md).[requestConfig](dijetscore.dijetscore-1.md#protected-requestconfig)*

*Defined in [src/dijets.ts:37](https://github.com/Dijets-Inc/dijetsjs/blob/ca67b81/src/dijets.ts#L37)*

___

### `Protected` url

• **url**: *string*

*Inherited from [DijetsCore](dijetscore.dijetscore-1.md).[url](dijetscore.dijetscore-1.md#protected-url)*

*Defined in [src/dijets.ts:34](https://github.com/Dijets-Inc/dijetsjs/blob/ca67b81/src/dijets.ts#L34)*

## Methods

###  Admin

▸ **Admin**(): *[AdminAPI](api_admin.adminapi.md)‹›*

*Defined in [src/index.ts:42](https://github.com/Dijets-Inc/dijetsjs/blob/ca67b81/src/index.ts#L42)*

Returns a reference to the Admin RPC.

**Returns:** *[AdminAPI](api_admin.adminapi.md)‹›*

___

###  Auth

▸ **Auth**(): *[AuthAPI](api_auth.authapi.md)‹›*

*Defined in [src/index.ts:47](https://github.com/Dijets-Inc/dijetsjs/blob/ca67b81/src/index.ts#L47)*

Returns a reference to the Auth RPC.

**Returns:** *[AuthAPI](api_auth.authapi.md)‹›*

___

###  CChain

▸ **CChain**(): *[EVMAPI](api_evm.evmapi.md)‹›*

*Defined in [src/index.ts:52](https://github.com/Dijets-Inc/dijetsjs/blob/ca67b81/src/index.ts#L52)*

Returns a reference to the EVMAPI RPC pointed at the C-Chain.

**Returns:** *[EVMAPI](api_evm.evmapi.md)‹›*

___

###  Health

▸ **Health**(): *[HealthAPI](api_health.healthapi.md)‹›*

*Defined in [src/index.ts:62](https://github.com/Dijets-Inc/dijetsjs/blob/ca67b81/src/index.ts#L62)*

Returns a reference to the Health RPC for a node.

**Returns:** *[HealthAPI](api_health.healthapi.md)‹›*

___

###  Index

▸ **Index**(): *[IndexAPI](api_index.indexapi.md)‹›*

*Defined in [src/index.ts:67](https://github.com/Dijets-Inc/dijetsjs/blob/ca67b81/src/index.ts#L67)*

Returns a reference to the Index RPC for a node.

**Returns:** *[IndexAPI](api_index.indexapi.md)‹›*

___

###  Info

▸ **Info**(): *[InfoAPI](api_info.infoapi.md)‹›*

*Defined in [src/index.ts:72](https://github.com/Dijets-Inc/dijetsjs/blob/ca67b81/src/index.ts#L72)*

Returns a reference to the Info RPC for a node.

**Returns:** *[InfoAPI](api_info.infoapi.md)‹›*

___

###  Metrics

▸ **Metrics**(): *[MetricsAPI](api_metrics.metricsapi.md)‹›*

*Defined in [src/index.ts:77](https://github.com/Dijets-Inc/dijetsjs/blob/ca67b81/src/index.ts#L77)*

Returns a reference to the Metrics RPC.

**Returns:** *[MetricsAPI](api_metrics.metricsapi.md)‹›*

___

###  NodeKeys

▸ **NodeKeys**(): *[KeystoreAPI](api_keystore.keystoreapi.md)‹›*

*Defined in [src/index.ts:83](https://github.com/Dijets-Inc/dijetsjs/blob/ca67b81/src/index.ts#L83)*

Returns a reference to the Keystore RPC for a node. We label it "NodeKeys" to reduce
confusion about what it's accessing.

**Returns:** *[KeystoreAPI](api_keystore.keystoreapi.md)‹›*

___

###  PChain

▸ **PChain**(): *[PlatformVMAPI](api_platformvm.platformvmapi.md)‹›*

*Defined in [src/index.ts:88](https://github.com/Dijets-Inc/dijetsjs/blob/ca67b81/src/index.ts#L88)*

Returns a reference to the PlatformVM RPC pointed at the P-Chain.

**Returns:** *[PlatformVMAPI](api_platformvm.platformvmapi.md)‹›*

___

###  XChain

▸ **XChain**(): *[AVMAPI](api_avm.avmapi.md)‹›*

*Defined in [src/index.ts:57](https://github.com/Dijets-Inc/dijetsjs/blob/ca67b81/src/index.ts#L57)*

Returns a reference to the AVM RPC pointed at the X-Chain.

**Returns:** *[AVMAPI](api_avm.avmapi.md)‹›*

___

### `Protected` _setHeaders

▸ **_setHeaders**(`headers`: any): *AxiosRequestHeaders*

*Inherited from [DijetsCore](dijetscore.dijetscore-1.md).[_setHeaders](dijetscore.dijetscore-1.md#protected-_setheaders)*

*Defined in [src/dijets.ts:227](https://github.com/Dijets-Inc/dijetsjs/blob/ca67b81/src/dijets.ts#L227)*

**Parameters:**

Name | Type |
------ | ------ |
`headers` | any |

**Returns:** *AxiosRequestHeaders*

___

###  addAPI

▸ **addAPI**‹**GA**›(`apiName`: string, `ConstructorFN`: object, `baseurl`: string, ...`args`: any[]): *void*

*Inherited from [DijetsCore](dijetscore.dijetscore-1.md).[addAPI](dijetscore.dijetscore-1.md#addapi)*

*Defined in [src/dijets.ts:259](https://github.com/Dijets-Inc/dijetsjs/blob/ca67b81/src/dijets.ts#L259)*

Adds an API to the middleware. The API resolves to a registered blockchain's RPC.

In TypeScript:
```js
dijets.addAPI<MyVMClass>("mychain", MyVMClass, "/ext/bc/mychain")
```

In Javascript:
```js
dijets.addAPI("mychain", MyVMClass, "/ext/bc/mychain")
```

**Type parameters:**

▪ **GA**: *[APIBase](common_apibase.apibase.md)*

Class of the API being added

**Parameters:**

Name | Type | Default | Description |
------ | ------ | ------ | ------ |
`apiName` | string | - | A label for referencing the API in the future |
`ConstructorFN` | object | - | A reference to the class which instantiates the API |
`baseurl` | string | undefined | Path to resolve to reach the API   |
`...args` | any[] | - | - |

**Returns:** *void*

___

###  api

▸ **api**‹**GA**›(`apiName`: string): *GA*

*Inherited from [DijetsCore](dijetscore.dijetscore-1.md).[api](dijetscore.dijetscore-1.md#api)*

*Defined in [src/dijets.ts:281](https://github.com/Dijets-Inc/dijetsjs/blob/ca67b81/src/dijets.ts#L281)*

Retrieves a reference to an API by its apiName label.

**Type parameters:**

▪ **GA**: *[APIBase](common_apibase.apibase.md)*

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`apiName` | string | Name of the API to return  |

**Returns:** *GA*

___

###  delete

▸ **delete**(`baseurl`: string, `getdata`: object, `headers`: object, `axiosConfig`: AxiosRequestConfig): *Promise‹[RequestResponseData](common_apibase.requestresponsedata.md)›*

*Inherited from [DijetsCore](dijetscore.dijetscore-1.md).[delete](dijetscore.dijetscore-1.md#delete)*

*Defined in [src/dijets.ts:366](https://github.com/Dijets-Inc/dijetsjs/blob/ca67b81/src/dijets.ts#L366)*

Makes a DELETE call to an API.

**Parameters:**

Name | Type | Default | Description |
------ | ------ | ------ | ------ |
`baseurl` | string | - | Path to the API |
`getdata` | object | - | Object containing the key value pairs sent in DELETE |
`headers` | object | {} | An array HTTP Request Headers |
`axiosConfig` | AxiosRequestConfig | undefined | Configuration for the axios javascript library that will be the foundation for the rest of the parameters  |

**Returns:** *Promise‹[RequestResponseData](common_apibase.requestresponsedata.md)›*

A promise for [RequestResponseData](common_apibase.requestresponsedata.md)

___

###  get

▸ **get**(`baseurl`: string, `getdata`: object, `headers`: object, `axiosConfig`: AxiosRequestConfig): *Promise‹[RequestResponseData](common_apibase.requestresponsedata.md)›*

*Inherited from [DijetsCore](dijetscore.dijetscore-1.md).[get](dijetscore.dijetscore-1.md#get)*

*Defined in [src/dijets.ts:340](https://github.com/Dijets-Inc/dijetsjs/blob/ca67b81/src/dijets.ts#L340)*

Makes a GET call to an API.

**Parameters:**

Name | Type | Default | Description |
------ | ------ | ------ | ------ |
`baseurl` | string | - | Path to the api |
`getdata` | object | - | Object containing the key value pairs sent in GET |
`headers` | object | {} | An array HTTP Request Headers |
`axiosConfig` | AxiosRequestConfig | undefined | Configuration for the axios javascript library that will be the foundation for the rest of the parameters  |

**Returns:** *Promise‹[RequestResponseData](common_apibase.requestresponsedata.md)›*

A promise for [RequestResponseData](common_apibase.requestresponsedata.md)

___

###  getBaseEndpoint

▸ **getBaseEndpoint**(): *string*

*Inherited from [DijetsCore](dijetscore.dijetscore-1.md).[getBaseEndpoint](dijetscore.dijetscore-1.md#getbaseendpoint)*

*Defined in [src/dijets.ts:112](https://github.com/Dijets-Inc/dijetsjs/blob/ca67b81/src/dijets.ts#L112)*

Returns the base endpoint for the Dijets node.

**Returns:** *string*

___

###  getHRP

▸ **getHRP**(): *string*

*Inherited from [DijetsCore](dijetscore.dijetscore-1.md).[getHRP](dijetscore.dijetscore-1.md#gethrp)*

*Defined in [src/dijets.ts:147](https://github.com/Dijets-Inc/dijetsjs/blob/ca67b81/src/dijets.ts#L147)*

Returns the Human-Readable-Part of the network associated with this key.

**Returns:** *string*

The [KeyPair](api_evm_keychain.keypair.md)'s Human-Readable-Part of the network's Bech32 addressing scheme

___

###  getHeaders

▸ **getHeaders**(): *object*

*Inherited from [DijetsCore](dijetscore.dijetscore-1.md).[getHeaders](dijetscore.dijetscore-1.md#getheaders)*

*Defined in [src/dijets.ts:122](https://github.com/Dijets-Inc/dijetsjs/blob/ca67b81/src/dijets.ts#L122)*

Returns the custom headers

**Returns:** *object*

___

###  getHost

▸ **getHost**(): *string*

*Inherited from [DijetsCore](dijetscore.dijetscore-1.md).[getHost](dijetscore.dijetscore-1.md#gethost)*

*Defined in [src/dijets.ts:97](https://github.com/Dijets-Inc/dijetsjs/blob/ca67b81/src/dijets.ts#L97)*

Returns the host for the Dijets node.

**Returns:** *string*

___

###  getIP

▸ **getIP**(): *string*

*Inherited from [DijetsCore](dijetscore.dijetscore-1.md).[getIP](dijetscore.dijetscore-1.md#getip)*

*Defined in [src/dijets.ts:102](https://github.com/Dijets-Inc/dijetsjs/blob/ca67b81/src/dijets.ts#L102)*

Returns the IP for the Dijets node.

**Returns:** *string*

___

###  getNetworkID

▸ **getNetworkID**(): *number*

*Inherited from [DijetsCore](dijetscore.dijetscore-1.md).[getNetworkID](dijetscore.dijetscore-1.md#getnetworkid)*

*Defined in [src/dijets.ts:132](https://github.com/Dijets-Inc/dijetsjs/blob/ca67b81/src/dijets.ts#L132)*

Returns the networkID

**Returns:** *number*

___

###  getPort

▸ **getPort**(): *number*

*Inherited from [DijetsCore](dijetscore.dijetscore-1.md).[getPort](dijetscore.dijetscore-1.md#getport)*

*Defined in [src/dijets.ts:107](https://github.com/Dijets-Inc/dijetsjs/blob/ca67b81/src/dijets.ts#L107)*

Returns the port for the Dijets node.

**Returns:** *number*

___

###  getProtocol

▸ **getProtocol**(): *string*

*Inherited from [DijetsCore](dijetscore.dijetscore-1.md).[getProtocol](dijetscore.dijetscore-1.md#getprotocol)*

*Defined in [src/dijets.ts:92](https://github.com/Dijets-Inc/dijetsjs/blob/ca67b81/src/dijets.ts#L92)*

Returns the protocol such as "http", "https", "git", "ws", etc.

**Returns:** *string*

___

###  getRequestConfig

▸ **getRequestConfig**(): *AxiosRequestConfig*

*Inherited from [DijetsCore](dijetscore.dijetscore-1.md).[getRequestConfig](dijetscore.dijetscore-1.md#getrequestconfig)*

*Defined in [src/dijets.ts:127](https://github.com/Dijets-Inc/dijetsjs/blob/ca67b81/src/dijets.ts#L127)*

Returns the custom request config

**Returns:** *AxiosRequestConfig*

___

###  getURL

▸ **getURL**(): *string*

*Inherited from [DijetsCore](dijetscore.dijetscore-1.md).[getURL](dijetscore.dijetscore-1.md#geturl)*

*Defined in [src/dijets.ts:117](https://github.com/Dijets-Inc/dijetsjs/blob/ca67b81/src/dijets.ts#L117)*

Returns the URL of the Dijets node (ip + port)

**Returns:** *string*

___

###  patch

▸ **patch**(`baseurl`: string, `getdata`: object, `postdata`: string | object | ArrayBuffer | ArrayBufferView, `headers`: object, `axiosConfig`: AxiosRequestConfig): *Promise‹[RequestResponseData](common_apibase.requestresponsedata.md)›*

*Inherited from [DijetsCore](dijetscore.dijetscore-1.md).[patch](dijetscore.dijetscore-1.md#patch)*

*Defined in [src/dijets.ts:450](https://github.com/Dijets-Inc/dijetsjs/blob/ca67b81/src/dijets.ts#L450)*

Makes a PATCH call to an API.

**Parameters:**

Name | Type | Default | Description |
------ | ------ | ------ | ------ |
`baseurl` | string | - | Path to the baseurl |
`getdata` | object | - | Object containing the key value pairs sent in PATCH |
`postdata` | string &#124; object &#124; ArrayBuffer &#124; ArrayBufferView | - | Object containing the key value pairs sent in PATCH |
`headers` | object | {} | An array HTTP Request Headers |
`axiosConfig` | AxiosRequestConfig | undefined | Configuration for the axios javascript library that will be the foundation for the rest of the parameters  |

**Returns:** *Promise‹[RequestResponseData](common_apibase.requestresponsedata.md)›*

A promise for [RequestResponseData](common_apibase.requestresponsedata.md)

___

###  post

▸ **post**(`baseurl`: string, `getdata`: object, `postdata`: string | object | ArrayBuffer | ArrayBufferView, `headers`: object, `axiosConfig`: AxiosRequestConfig): *Promise‹[RequestResponseData](common_apibase.requestresponsedata.md)›*

*Inherited from [DijetsCore](dijetscore.dijetscore-1.md).[post](dijetscore.dijetscore-1.md#post)*

*Defined in [src/dijets.ts:393](https://github.com/Dijets-Inc/dijetsjs/blob/ca67b81/src/dijets.ts#L393)*

Makes a POST call to an API.

**Parameters:**

Name | Type | Default | Description |
------ | ------ | ------ | ------ |
`baseurl` | string | - | Path to the API |
`getdata` | object | - | Object containing the key value pairs sent in POST |
`postdata` | string &#124; object &#124; ArrayBuffer &#124; ArrayBufferView | - | Object containing the key value pairs sent in POST |
`headers` | object | {} | An array HTTP Request Headers |
`axiosConfig` | AxiosRequestConfig | undefined | Configuration for the axios javascript library that will be the foundation for the rest of the parameters  |

**Returns:** *Promise‹[RequestResponseData](common_apibase.requestresponsedata.md)›*

A promise for [RequestResponseData](common_apibase.requestresponsedata.md)

___

###  put

▸ **put**(`baseurl`: string, `getdata`: object, `postdata`: string | object | ArrayBuffer | ArrayBufferView, `headers`: object, `axiosConfig`: AxiosRequestConfig): *Promise‹[RequestResponseData](common_apibase.requestresponsedata.md)›*

*Inherited from [DijetsCore](dijetscore.dijetscore-1.md).[put](dijetscore.dijetscore-1.md#put)*

*Defined in [src/dijets.ts:421](https://github.com/Dijets-Inc/dijetsjs/blob/ca67b81/src/dijets.ts#L421)*

Makes a PUT call to an API.

**Parameters:**

Name | Type | Default | Description |
------ | ------ | ------ | ------ |
`baseurl` | string | - | Path to the baseurl |
`getdata` | object | - | Object containing the key value pairs sent in PUT |
`postdata` | string &#124; object &#124; ArrayBuffer &#124; ArrayBufferView | - | Object containing the key value pairs sent in PUT |
`headers` | object | {} | An array HTTP Request Headers |
`axiosConfig` | AxiosRequestConfig | undefined | Configuration for the axios javascript library that will be the foundation for the rest of the parameters  |

**Returns:** *Promise‹[RequestResponseData](common_apibase.requestresponsedata.md)›*

A promise for [RequestResponseData](common_apibase.requestresponsedata.md)

___

###  removeAllHeaders

▸ **removeAllHeaders**(): *void*

*Inherited from [DijetsCore](dijetscore.dijetscore-1.md).[removeAllHeaders](dijetscore.dijetscore-1.md#removeallheaders)*

*Defined in [src/dijets.ts:180](https://github.com/Dijets-Inc/dijetsjs/blob/ca67b81/src/dijets.ts#L180)*

Removes all headers.

**Returns:** *void*

___

###  removeAllRequestConfigs

▸ **removeAllRequestConfigs**(): *void*

*Inherited from [DijetsCore](dijetscore.dijetscore-1.md).[removeAllRequestConfigs](dijetscore.dijetscore-1.md#removeallrequestconfigs)*

*Defined in [src/dijets.ts:210](https://github.com/Dijets-Inc/dijetsjs/blob/ca67b81/src/dijets.ts#L210)*

Removes all request configs.

**Returns:** *void*

___

###  removeHeader

▸ **removeHeader**(`key`: string): *void*

*Inherited from [DijetsCore](dijetscore.dijetscore-1.md).[removeHeader](dijetscore.dijetscore-1.md#removeheader)*

*Defined in [src/dijets.ts:173](https://github.com/Dijets-Inc/dijetsjs/blob/ca67b81/src/dijets.ts#L173)*

Removes a previously added custom header.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`key` | string | Header name  |

**Returns:** *void*

___

###  removeRequestConfig

▸ **removeRequestConfig**(`key`: string): *void*

*Inherited from [DijetsCore](dijetscore.dijetscore-1.md).[removeRequestConfig](dijetscore.dijetscore-1.md#removerequestconfig)*

*Defined in [src/dijets.ts:203](https://github.com/Dijets-Inc/dijetsjs/blob/ca67b81/src/dijets.ts#L203)*

Removes a previously added request config.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`key` | string | Header name  |

**Returns:** *void*

___

###  setAddress

▸ **setAddress**(`host`: string, `port`: number, `protocol`: string, `baseEndpoint`: string): *void*

*Inherited from [DijetsCore](dijetscore.dijetscore-1.md).[setAddress](dijetscore.dijetscore-1.md#setaddress)*

*Defined in [src/dijets.ts:52](https://github.com/Dijets-Inc/dijetsjs/blob/ca67b81/src/dijets.ts#L52)*

Sets the address and port of the main Dijets Client.

**Parameters:**

Name | Type | Default | Description |
------ | ------ | ------ | ------ |
`host` | string | - | The hostname to resolve to reach the Dijets Client RPC APIs. |
`port` | number | - | The port to resolve to reach the Dijets Client RPC APIs. |
`protocol` | string | "http" | The protocol string to use before a "://" in a request, ex: "http", "https", etc. Defaults to http |
`baseEndpoint` | string | "" | the base endpoint to reach the Dijets Client RPC APIs, ex: "/rpc". Defaults to "/" The following special characters are removed from host and protocol &#,@+()$~%'":*?{} also less than and greater than signs  |

**Returns:** *void*

___

###  setAuthToken

▸ **setAuthToken**(`auth`: string): *void*

*Inherited from [DijetsCore](dijetscore.dijetscore-1.md).[setAuthToken](dijetscore.dijetscore-1.md#setauthtoken)*

*Defined in [src/dijets.ts:223](https://github.com/Dijets-Inc/dijetsjs/blob/ca67b81/src/dijets.ts#L223)*

Sets the temporary auth token used for communicating with the node.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`auth` | string | A temporary token provided by the node enabling access to the endpoints on the node.  |

**Returns:** *void*

___

###  setHRP

▸ **setHRP**(`hrp`: string): *void*

*Inherited from [DijetsCore](dijetscore.dijetscore-1.md).[setHRP](dijetscore.dijetscore-1.md#sethrp)*

*Defined in [src/dijets.ts:154](https://github.com/Dijets-Inc/dijetsjs/blob/ca67b81/src/dijets.ts#L154)*

Sets the the Human-Readable-Part of the network associated with this key.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`hrp` | string | String for the Human-Readable-Part of Bech32 addresses  |

**Returns:** *void*

___

###  setHeader

▸ **setHeader**(`key`: string, `value`: string): *void*

*Inherited from [DijetsCore](dijetscore.dijetscore-1.md).[setHeader](dijetscore.dijetscore-1.md#setheader)*

*Defined in [src/dijets.ts:164](https://github.com/Dijets-Inc/dijetsjs/blob/ca67b81/src/dijets.ts#L164)*

Adds a new custom header to be included with all requests.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`key` | string | Header name |
`value` | string | Header value  |

**Returns:** *void*

___

###  setNetworkID

▸ **setNetworkID**(`netID`: number): *void*

*Inherited from [DijetsCore](dijetscore.dijetscore-1.md).[setNetworkID](dijetscore.dijetscore-1.md#setnetworkid)*

*Defined in [src/dijets.ts:137](https://github.com/Dijets-Inc/dijetsjs/blob/ca67b81/src/dijets.ts#L137)*

Sets the networkID

**Parameters:**

Name | Type |
------ | ------ |
`netID` | number |

**Returns:** *void*

___

###  setRequestConfig

▸ **setRequestConfig**(`key`: string, `value`: string | boolean): *void*

*Inherited from [DijetsCore](dijetscore.dijetscore-1.md).[setRequestConfig](dijetscore.dijetscore-1.md#setrequestconfig)*

*Defined in [src/dijets.ts:194](https://github.com/Dijets-Inc/dijetsjs/blob/ca67b81/src/dijets.ts#L194)*

Adds a new custom config value to be included with all requests.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`key` | string | Config name |
`value` | string &#124; boolean | Config value  |

**Returns:** *void*
