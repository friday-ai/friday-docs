**friday-server**

> [README](../README.md) / [Globals](../globals.md) / user

# Module: user

## Index

### Classes

* [User](../classes/user.user-1.md)

### Interfaces

* [UserType](../interfaces/user.usertype.md)

### Functions

* [create](user.md#create)
* [destroy](user.md#destroy)
* [getAll](user.md#getall)
* [getById](user.md#getbyid)
* [getCount](user.md#getcount)
* [update](user.md#update)

## Functions

### create

▸ **create**(`user`: [UserType](../interfaces/user.usertype.md)): Promise\<[UserType](../interfaces/user.usertype.md)>

*Defined in [src/core/user/user.create.ts:23](https://github.com/friday-ai/friday/blob/cd1d9b5/server/src/core/user/user.create.ts#L23)*

Create a user.

**`example`** 
````
friday.user.create({
   id: '87d636b2-fa65-4f0e-ae04-622562f62c31',
   name: 'Pepperwood',
   firstName: 'John',
   email: 'sample@sample.com',
   password: 'mysupersamplepassword',
   birthDate: new Date(1996, 12, 20)
});
````

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`user` | [UserType](../interfaces/user.usertype.md) | A user object. |

**Returns:** Promise\<[UserType](../interfaces/user.usertype.md)>

Resolve with created user.

___

### destroy

▸ **destroy**(`id`: string): Promise\<void>

*Defined in [src/core/user/user.destroy.ts:13](https://github.com/friday-ai/friday/blob/cd1d9b5/server/src/core/user/user.destroy.ts#L13)*

Destroy a user.

**`example`** 
````
friday.user.destroy('e8768abf-f6c9-4689-9ca4-2fe663e4ce9f');
````

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`id` | string | Id of user. |

**Returns:** Promise\<void>

___

### getAll

▸ **getAll**(`options?`: GetOptions): Promise\<[UserType](../interfaces/user.usertype.md)[]>

*Defined in [src/core/user/user.getAll.ts:25](https://github.com/friday-ai/friday/blob/cd1d9b5/server/src/core/user/user.getAll.ts#L25)*

GEt all users.

**`example`** 
````
friday.user.getAll({
   scope: '',
   take: 20,
   skip: 0
 });
````

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`options?` | GetOptions | Options of the query. |

**Returns:** Promise\<[UserType](../interfaces/user.usertype.md)[]>

Resolve with user array.

___

### getById

▸ **getById**(`id`: string, `scope?`: undefined \| string): Promise\<[UserType](../interfaces/user.usertype.md)>

*Defined in [src/core/user/user.getById.ts:15](https://github.com/friday-ai/friday/blob/cd1d9b5/server/src/core/user/user.getById.ts#L15)*

Get a user by id.

**`example`** 
````
friday.user.getById('a8ba342e-854a-4906-8670-d400c868bdb1', 'full');
````

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`id` | string | Id of user. |
`scope?` | undefined \| string | Scope option. (Optional) |

**Returns:** Promise\<[UserType](../interfaces/user.usertype.md)>

Resolve with user.

___

### getCount

▸ **getCount**(): Promise\<number>

*Defined in [src/core/user/user.getCount.ts:12](https://github.com/friday-ai/friday/blob/cd1d9b5/server/src/core/user/user.getCount.ts#L12)*

Get count of users.

**`example`** 
````
friday.user.getCount();
````

**Returns:** Promise\<number>

Resolve with number of users.

___

### update

▸ **update**(`id`: string, `user`: [UserType](../interfaces/user.usertype.md)): Promise\<[UserType](../interfaces/user.usertype.md)>

*Defined in [src/core/user/user.update.ts:20](https://github.com/friday-ai/friday/blob/cd1d9b5/server/src/core/user/user.update.ts#L20)*

Update a user.

**`example`** 
````
friday.user.update(
'f8be3bad-3d46-4009-b965-fe03a4d6d5f1',
{
  id: 'f8be3bad-3d46-4009-b965-fe03a4d6d5f1'
  name: 'user update'
});
````

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`id` | string | Id of user |
`user` | [UserType](../interfaces/user.usertype.md) | A user object. |

**Returns:** Promise\<[UserType](../interfaces/user.usertype.md)>

Resolve with updated user.
