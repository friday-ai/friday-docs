**friday-server**

> [README](../README.md) / [Globals](../globals.md) / session

# Module: session

## Index

### Classes

* [Session](../classes/session.session-1.md)

### Interfaces

* [AccessTokenType](../interfaces/session.accesstokentype.md)
* [SessionType](../interfaces/session.sessiontype.md)

### Functions

* [create](session.md#create)
* [getAccessToken](session.md#getaccesstoken)
* [getAll](session.md#getall)
* [getById](session.md#getbyid)
* [revoke](session.md#revoke)
* [validateAccessToken](session.md#validateaccesstoken)
* [validateRefreshToken](session.md#validaterefreshtoken)

## Functions

### create

▸ **create**(`this`: SessionClass, `user`: [UserType](../interfaces/user.usertype.md)): Promise\<[SessionType](../interfaces/session.sessiontype.md)>

*Defined in [src/core/session/session.create.ts:25](https://github.com/friday-ai/friday/blob/cd1d9b5/server/src/core/session/session.create.ts#L25)*

Create an session.

**`example`** 
````
friday.session.create({
   id: '87d636b2-fa65-4f0e-ae04-622562f62c31',
   name: 'Pepperwood',
   firstName: 'John',
   email: 'sample@sample.com',
   password: 'mysupersamplepassword',
   birthDate: new Date(1996, 12, 20),
   role: 'admin'
});
````

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`this` | SessionClass | - |
`user` | [UserType](../interfaces/user.usertype.md) | A user object. |

**Returns:** Promise\<[SessionType](../interfaces/session.sessiontype.md)>

Resolve with created session.

___

### getAccessToken

▸ **getAccessToken**(`this`: SessionClass, `refreshToken`: string): Promise\<[SessionType](../interfaces/session.sessiontype.md)>

*Defined in [src/core/session/session.getAccessToken.ts:13](https://github.com/friday-ai/friday/blob/cd1d9b5/server/src/core/session/session.getAccessToken.ts#L13)*

Get a new access token.

**`example`** 
friday.session.getAccessToken('test');

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`this` | SessionClass | - |
`refreshToken` | string | The refresh token to verify. |

**Returns:** Promise\<[SessionType](../interfaces/session.sessiontype.md)>

Resolve with an session object.

___

### getAll

▸ **getAll**(`options?`: GetOptions): Promise\<[SessionType](../interfaces/session.sessiontype.md)[]>

*Defined in [src/core/session/session.getAll.ts:25](https://github.com/friday-ai/friday/blob/cd1d9b5/server/src/core/session/session.getAll.ts#L25)*

Get all sessions.

**`example`** 
````
friday.session.getAll({
   scope: '',
   take: 20,
   skip: 0
 });
````

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`options?` | GetOptions | Options of the query. |

**Returns:** Promise\<[SessionType](../interfaces/session.sessiontype.md)[]>

Resolve with session array.

___

### getById

▸ **getById**(`id`: string, `scope?`: undefined \| string): Promise\<[SessionType](../interfaces/session.sessiontype.md)>

*Defined in [src/core/session/session.getById.ts:15](https://github.com/friday-ai/friday/blob/cd1d9b5/server/src/core/session/session.getById.ts#L15)*

Get an session by id.

**`example`** 
````
friday.session.getById('a8ba342e-854a-4906-8670-d400c868bdb1', 'full');
````

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`id` | string | Id of session. |
`scope?` | undefined \| string | Scope option. (Optional) |

**Returns:** Promise\<[SessionType](../interfaces/session.sessiontype.md)>

Resolve with session.

___

### revoke

▸ **revoke**(`userId`: string, `sessionId`: string): Promise\<[SessionType](../interfaces/session.sessiontype.md)>

*Defined in [src/core/session/session.revoke.ts:15](https://github.com/friday-ai/friday/blob/cd1d9b5/server/src/core/session/session.revoke.ts#L15)*

Revoke an session.

**`example`** 
````
friday.session.revoke('a8ba342e-854a-4906-8670-d400c868bdb1', 'b991aa73-2acb-4e24-8f95-66fbd27506b6');
````

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`userId` | string | Id of user. |
`sessionId` | string | Id of session. |

**Returns:** Promise\<[SessionType](../interfaces/session.sessiontype.md)>

Resolve with session revoked.

___

### validateAccessToken

▸ **validateAccessToken**(`this`: SessionClass, `accessToken`: string): Promise\<[AccessTokenType](../interfaces/session.accesstokentype.md)>

*Defined in [src/core/session/session.validateAccessToken.ts:13](https://github.com/friday-ai/friday/blob/cd1d9b5/server/src/core/session/session.validateAccessToken.ts#L13)*

Validate access token

**`example`** 
friday.session.validateAccessToken('test');

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`this` | SessionClass | - |
`accessToken` | string | The access token to verify. |

**Returns:** Promise\<[AccessTokenType](../interfaces/session.accesstokentype.md)>

Resolve with a access token object.

___

### validateRefreshToken

▸ **validateRefreshToken**(`refreshToken`: string, `scope?`: undefined \| string): Promise\<[SessionType](../interfaces/session.sessiontype.md)>

*Defined in [src/core/session/session.validateRefreshToken.ts:15](https://github.com/friday-ai/friday/blob/cd1d9b5/server/src/core/session/session.validateRefreshToken.ts#L15)*

Validate refresh token

**`description`** Validate a refresh token.

**`example`** 
friday.session.validateRefreshToken('test');

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`refreshToken` | string | The refresh token to verify. |
`scope?` | undefined \| string | Scope option. (Optional) |

**Returns:** Promise\<[SessionType](../interfaces/session.sessiontype.md)>

Resolve with an session object.
