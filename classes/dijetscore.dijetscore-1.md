[dijets](../README.md) › [DijetsCore](../modules/dijetscore.md) › [DijetsCore](dijetscore.dijetscore-1.md)

# Class: DijetsCore

DijetsCore is middleware for interacting with Dijets node RPC APIs.

Example usage:
```js
let dijets = new DijetsCore("127.0.0.1", 9650, "https")
```

## Hierarchy

* **DijetsCore**

  ↳ [Dijets](dijets.dijets-1.md)

## Index

### Constructors

* [constructor](dijetscore.dijetscore-1.md#constructor)

### Properties

* [apis](dijetscore.dijetscore-1.md#protected-apis)
* [auth](dijetscore.dijetscore-1.md#protected-auth)
* [baseEndpoint](dijetscore.dijetscore-1.md#protected-baseendpoint)
* [headers](dijetscore.dijetscore-1.md#protected-headers)
* [host](dijetscore.dijetscore-1.md#protected-host)
* [hrp](dijetscore.dijetscore-1.md#protected-hrp)
* [ip](dijetscore.dijetscore-1.md#protected-ip)
* [networkID](dijetscore.dijetscore-1.md#protected-networkid)
* [port](dijetscore.dijetscore-1.md#protected-port)
* [protocol](dijetscore.dijetscore-1.md#protected-protocol)
* [requestConfig](dijetscore.dijetscore-1.md#protected-requestconfig)
* [url](dijetscore.dijetscore-1.md#protected-url)

### Methods

* [_setHeaders](dijetscore.dijetscore-1.md#protected-_setheaders)
* [addAPI](dijetscore.dijetscore-1.md#addapi)
* [api](dijetscore.dijetscore-1.md#api)
* [delete](dijetscore.dijetscore-1.md#delete)
* [get](dijetscore.dijetscore-1.md#get)
* [getBaseEndpoint](dijetscore.dijetscore-1.md#getbaseendpoint)
* [getHRP](dijetscore.dijetscore-1.md#gethrp)
* [getHeaders](dijetscore.dijetscore-1.md#getheaders)
* [getHost](dijetscore.dijetscore-1.md#gethost)
* [getIP](dijetscore.dijetscore-1.md#getip)
* [getNetworkID](dijetscore.dijetscore-1.md#getnetworkid)
* [getPort](dijetscore.dijetscore-1.md#getport)
* [getProtocol](dijetscore.dijetscore-1.md#getprotocol)
* [getRequestConfig](dijetscore.dijetscore-1.md#getrequestconfig)
* [getURL](dijetscore.dijetscore-1.md#geturl)
* [patch](dijetscore.dijetscore-1.md#patch)
* [post](dijetscore.dijetscore-1.md#post)
* [put](dijetscore.dijetscore-1.md#put)
* [removeAllHeaders](dijetscore.dijetscore-1.md#removeallheaders)
* [removeAllRequestConfigs](dijetscore.dijetscore-1.md#removeallrequestconfigs)
* [removeHeader](dijetscore.dijetscore-1.md#removeheader)
* [removeRequestConfig](dijetscore.dijetscore-1.md#removerequestconfig)
* [setAddress](dijetscore.dijetscore-1.md#setaddress)
* [setAuthToken](dijetscore.dijetscore-1.md#setauthtoken)
* [setHRP](dijetscore.dijetscore-1.md#sethrp)
* [setHeader](dijetscore.dijetscore-1.md#setheader)
* [setNetworkID](dijetscore.dijetscore-1.md#setnetworkid)
* [setRequestConfig](dijetscore.dijetscore-1.md#setrequestconfig)

## Constructors

###  constructor

\+ **new DijetsCore**(`host?`: string, `port?`: number, `protocol`: string): *[DijetsCore](dijetscore.dijetscore-1.md)*

*Defined in [src/dijets.ts:464](https://github.com/Dijets-Inc/dijetsjs/blob/master/src/dijets.ts#L464)*

Creates a new Dijets instance. Sets the address and port of the main Dijets Client.

**Parameters:**

Name | Type | Default | Description |
------ | ------ | ------ | ------ |
`host?` | string | - | The hostname to resolve to reach the Dijets Client APIs |
`port?` | number | - | The port to resolve to reach the Dijets Client APIs |
`protocol` | string | "http" | The protocol string to use before a "://" in a request, ex: "http", "https", "git", "ws", etc ...  |

**Returns:** *[DijetsCore](dijetscore.dijetscore-1.md)*

## Properties

### `Protected` apis

• **apis**: *object*

*Defined in [src/dijets.ts:38](https://github.com/Dijets-Inc/dijetsjs/blob/master/src/dijets.ts#L38)*

#### Type declaration:

* \[ **k**: *string*\]: [APIBase](common_apibase.apibase.md)

___

### `Protected` auth

• **auth**: *string* = undefined

*Defined in [src/dijets.ts:35](https://github.com/Dijets-Inc/dijetsjs/blob/master/src/dijets.ts#L35)*

___

### `Protected` baseEndpoint

• **baseEndpoint**: *string*

*Defined in [src/dijets.ts:33](https://github.com/Dijets-Inc/dijetsjs/blob/master/src/dijets.ts#L33)*

___

### `Protected` headers

• **headers**: *object*

*Defined in [src/dijets.ts:36](https://github.com/Dijets-Inc/dijetsjs/blob/master/src/dijets.ts#L36)*

#### Type declaration:

* \[ **k**: *string*\]: string

___

### `Protected` host

• **host**: *string*

*Defined in [src/dijets.ts:31](https://github.com/Dijets-Inc/dijetsjs/blob/master/src/dijets.ts#L31)*

___

### `Protected` hrp

• **hrp**: *string* = ""

*Defined in [src/dijets.ts:28](https://github.com/Dijets-Inc/dijetsjs/blob/master/src/dijets.ts#L28)*

___

### `Protected` ip

• **ip**: *string*

*Defined in [src/dijets.ts:30](https://github.com/Dijets-Inc/dijetsjs/blob/master/src/dijets.ts#L30)*

___

### `Protected` networkID

• **networkID**: *number* = 0

*Defined in [src/dijets.ts:27](https://github.com/Dijets-Inc/dijetsjs/blob/master/src/dijets.ts#L27)*

___

### `Protected` port

• **port**: *number*

*Defined in [src/dijets.ts:32](https://github.com/Dijets-Inc/dijetsjs/blob/master/src/dijets.ts#L32)*

___

### `Protected` protocol

• **protocol**: *string*

*Defined in [src/dijets.ts:29](https://github.com/Dijets-Inc/dijetsjs/blob/master/src/dijets.ts#L29)*

___

### `Protected` requestConfig

• **requestConfig**: *AxiosRequestConfig*

*Defined in [src/dijets.ts:37](https://github.com/Dijets-Inc/dijetsjs/blob/master/src/dijets.ts#L37)*

___

### `Protected` url

• **url**: *string*

*Defined in [src/dijets.ts:34](https://github.com/Dijets-Inc/dijetsjs/blob/master/src/dijets.ts#L34)*

## Methods

### `Protected` _setHeaders

▸ **_setHeaders**(`headers`: any): *AxiosRequestHeaders*

*Defined in [src/dijets.ts:227](https://github.com/Dijets-Inc/dijetsjs/blob/master/src/dijets.ts#L227)*

**Parameters:**

Name | Type |
------ | ------ |
`headers` | any |

**Returns:** *AxiosRequestHeaders*

___

###  addAPI

▸ **addAPI**‹**GA**›(`apiName`: string, `ConstructorFN`: object, `baseurl`: string, ...`args`: any[]): *void*

*Defined in [src/dijets.ts:259](https://github.com/Dijets-Inc/dijetsjs/blob/master/src/dijets.ts#L259)*

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

*Defined in [src/dijets.ts:281](https://github.com/Dijets-Inc/dijetsjs/blob/master/src/dijets.ts#L281)*

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

*Defined in [src/dijets.ts:366](https://github.com/Dijets-Inc/dijetsjs/blob/master/src/dijets.ts#L366)*

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

*Defined in [src/dijets.ts:340](https://github.com/Dijets-Inc/dijetsjs/blob/master/src/dijets.ts#L340)*

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

*Defined in [src/dijets.ts:112](https://github.com/Dijets-Inc/dijetsjs/blob/master/src/dijets.ts#L112)*

Returns the base endpoint for the Dijets node.

**Returns:** *string*

___

###  getHRP

▸ **getHRP**(): *string*

*Defined in [src/dijets.ts:147](https://github.com/Dijets-Inc/dijetsjs/blob/master/src/dijets.ts#L147)*

Returns the Human-Readable-Part of the network associated with this key.

**Returns:** *string*

The [KeyPair](api_evm_keychain.keypair.md)'s Human-Readable-Part of the network's Bech32 addressing scheme

___

###  getHeaders

▸ **getHeaders**(): *object*

*Defined in [src/dijets.ts:122](https://github.com/Dijets-Inc/dijetsjs/blob/master/src/dijets.ts#L122)*

Returns the custom headers

**Returns:** *object*

___

###  getHost

▸ **getHost**(): *string*

*Defined in [src/dijets.ts:97](https://github.com/Dijets-Inc/dijetsjs/blob/master/src/dijets.ts#L97)*

Returns the host for the Dijets node.

**Returns:** *string*

___

###  getIP

▸ **getIP**(): *string*

*Defined in [src/dijets.ts:102](https://github.com/Dijets-Inc/dijetsjs/blob/master/src/dijets.ts#L102)*

Returns the IP for the Dijets node.

**Returns:** *string*

___

###  getNetworkID

▸ **getNetworkID**(): *number*

*Defined in [src/dijets.ts:132](https://github.com/Dijets-Inc/dijetsjs/blob/master/src/dijets.ts#L132)*

Returns the networkID

**Returns:** *number*

___

###  getPort

▸ **getPort**(): *number*

*Defined in [src/dijets.ts:107](https://github.com/Dijets-Inc/dijetsjs/blob/master/src/dijets.ts#L107)*

Returns the port for the Dijets node.

**Returns:** *number*

___

###  getProtocol

▸ **getProtocol**(): *string*

*Defined in [src/dijets.ts:92](https://github.com/Dijets-Inc/dijetsjs/blob/master/src/dijets.ts#L92)*

Returns the protocol such as "http", "https", "git", "ws", etc.

**Returns:** *string*

___

###  getRequestConfig

▸ **getRequestConfig**(): *AxiosRequestConfig*

*Defined in [src/dijets.ts:127](https://github.com/Dijets-Inc/dijetsjs/blob/master/src/dijets.ts#L127)*

Returns the custom request config

**Returns:** *AxiosRequestConfig*

___

###  getURL

▸ **getURL**(): *string*

*Defined in [src/dijets.ts:117](https://github.com/Dijets-Inc/dijetsjs/blob/master/src/dijets.ts#L117)*

Returns the URL of the Dijets node (ip + port)

**Returns:** *string*

___

###  patch

▸ **patch**(`baseurl`: string, `getdata`: object, `postdata`: string | object | ArrayBuffer | ArrayBufferView, `headers`: object, `axiosConfig`: AxiosRequestConfig): *Promise‹[RequestResponseData](common_apibase.requestresponsedata.md)›*

*Defined in [src/dijets.ts:450](https://github.com/Dijets-Inc/dijetsjs/blob/master/src/dijets.ts#L450)*

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

*Defined in [src/dijets.ts:393](https://github.com/Dijets-Inc/dijetsjs/blob/master/src/dijets.ts#L393)*

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

*Defined in [src/dijets.ts:421](https://github.com/Dijets-Inc/dijetsjs/blob/master/src/dijets.ts#L421)*

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

*Defined in [src/dijets.ts:180](https://github.com/Dijets-Inc/dijetsjs/blob/master/src/dijets.ts#L180)*

Removes all headers.

**Returns:** *void*

___

###  removeAllRequestConfigs

▸ **removeAllRequestConfigs**(): *void*

*Defined in [src/dijets.ts:210](https://github.com/Dijets-Inc/dijetsjs/blob/master/src/dijets.ts#L210)*

Removes all request configs.

**Returns:** *void*

___

###  removeHeader

▸ **removeHeader**(`key`: string): *void*

*Defined in [src/dijets.ts:173](https://github.com/Dijets-Inc/dijetsjs/blob/master/src/dijets.ts#L173)*

Removes a previously added custom header.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`key` | string | Header name  |

**Returns:** *void*

___

###  removeRequestConfig

▸ **removeRequestConfig**(`key`: string): *void*

*Defined in [src/dijets.ts:203](https://github.com/Dijets-Inc/dijetsjs/blob/master/src/dijets.ts#L203)*

Removes a previously added request config.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`key` | string | Header name  |

**Returns:** *void*

___

###  setAddress

▸ **setAddress**(`host`: string, `port`: number, `protocol`: string, `baseEndpoint`: string): *void*

*Defined in [src/dijets.ts:52](https://github.com/Dijets-Inc/dijetsjs/blob/master/src/dijets.ts#L52)*

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

*Defined in [src/dijets.ts:223](https://github.com/Dijets-Inc/dijetsjs/blob/master/src/dijets.ts#L223)*

Sets the temporary auth token used for communicating with the node.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`auth` | string | A temporary token provided by the node enabling access to the endpoints on the node.  |

**Returns:** *void*

___

###  setHRP

▸ **setHRP**(`hrp`: string): *void*

*Defined in [src/dijets.ts:154](https://github.com/Dijets-Inc/dijetsjs/blob/master/src/dijets.ts#L154)*

Sets the the Human-Readable-Part of the network associated with this key.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`hrp` | string | String for the Human-Readable-Part of Bech32 addresses  |

**Returns:** *void*

___

###  setHeader

▸ **setHeader**(`key`: string, `value`: string): *void*

*Defined in [src/dijets.ts:164](https://github.com/Dijets-Inc/dijetsjs/blob/master/src/dijets.ts#L164)*

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

*Defined in [src/dijets.ts:137](https://github.com/Dijets-Inc/dijetsjs/blob/master/src/dijets.ts#L137)*

Sets the networkID

**Parameters:**

Name | Type |
------ | ------ |
`netID` | number |

**Returns:** *void*

___

###  setRequestConfig

▸ **setRequestConfig**(`key`: string, `value`: string | boolean): *void*

*Defined in [src/dijets.ts:194](https://github.com/Dijets-Inc/dijetsjs/blob/master/src/dijets.ts#L194)*

Adds a new custom config value to be included with all requests.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`key` | string | Config name |
`value` | string &#124; boolean | Config value  |

**Returns:** *void*
