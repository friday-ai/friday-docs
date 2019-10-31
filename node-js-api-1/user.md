# user

> [**friday-server**](./)

[Globals](https://github.com/friday-ai/friday-docs/tree/7469fd0637aa28a674d6c68645188ee863701e30/node-js-api-1/globals.md) / [user](user.md) /

## External module: user

#### Index

**Classes**

* [User](https://github.com/friday-ai/friday-docs/tree/7469fd0637aa28a674d6c68645188ee863701e30/node-js-api-1/classes/user.user-1.md)

**Interfaces**

* [UserType](https://github.com/friday-ai/friday-docs/tree/7469fd0637aa28a674d6c68645188ee863701e30/node-js-api-1/interfaces/user.usertype.md)

**Functions**

* [create](user.md#create)
* [destroy](user.md#destroy)
* [getAll](user.md#getall)
* [getById](user.md#getbyid)
* [update](user.md#update)

### Functions

#### create

▸ **create**\(`user`: [UserType](https://github.com/friday-ai/friday-docs/tree/7469fd0637aa28a674d6c68645188ee863701e30/node-js-api-1/interfaces/user.usertype.md)\): _`Promise<UserType>`_

Defined in user/user.create.ts:22

Create a user.

**`example`**

```text
friday.user.create({
   id: '87d636b2-fa65-4f0e-ae04-622562f62c31',
   name: 'Pepperwood',
   firstName: 'John',
   email: 'sample@sample.com',
   password: 'mysupersamplepassword',
   birthDate: new Date(1996, 12, 20)
});
```

**Parameters:**

| Name | Type | Description |
| :--- | :--- | :--- |
| `user` | [UserType](https://github.com/friday-ai/friday-docs/tree/7469fd0637aa28a674d6c68645188ee863701e30/node-js-api-1/interfaces/user.usertype.md) | A user object. |

**Returns:** _`Promise<UserType>`_

Resolve with created user.

#### destroy

▸ **destroy**\(`id`: string\): _`Promise<void>`_

Defined in user/user.destroy.ts:14

Destroy a user.

**`example`**

```text
friday.user.destroy('e8768abf-f6c9-4689-9ca4-2fe663e4ce9f');
```

**Parameters:**

| Name | Type | Description |
| :--- | :--- | :--- |
| `id` | string | Id of user. |

**Returns:** _`Promise<void>`_

#### getAll

▸ **getAll**\(`options?`: `GetOptions`\): _`Promise<UserType[]>`_

Defined in user/user.getAll.ts:26

GEt all users.

**`example`**

```text
friday.user.getAll({
   scope: '',
   take: 20,
   skip: 0
 });
```

**Parameters:**

| Name | Type | Description |
| :--- | :--- | :--- |
| `options?` | `GetOptions` | Options of the query. |

**Returns:** _`Promise<UserType[]>`_

Resolve with user array.

#### getById

▸ **getById**\(`id`: string, `scope?`: undefined \| string\): _`Promise<UserType>`_

Defined in user/user.getById.ts:17

Get a user by id.

**`example`**

```text
friday.user.getById('a8ba342e-854a-4906-8670-d400c868bdb1', 'full');
```

**Parameters:**

| Name | Type | Description |
| :--- | :--- | :--- |
| `id` | string | Id of user. |
| `scope?` | undefined \| string | Scope option. \(Optional\) |

**Returns:** _`Promise<UserType>`_

Resolve with user.

#### update

▸ **update**\(`user`: [UserType](https://github.com/friday-ai/friday-docs/tree/7469fd0637aa28a674d6c68645188ee863701e30/node-js-api-1/interfaces/user.usertype.md)\): _`Promise<UserType>`_

Defined in user/user.update.ts:18

Update a user.

**`example`**

```text
friday.user.update({
  id: 'f8be3bad-3d46-4009-b965-fe03a4d6d5f1'
  name: 'user update'
});
```

**Parameters:**

| Name | Type | Description |
| :--- | :--- | :--- |
| `user` | [UserType](https://github.com/friday-ai/friday-docs/tree/7469fd0637aa28a674d6c68645188ee863701e30/node-js-api-1/interfaces/user.usertype.md) | A user object. |

**Returns:** _`Promise<UserType>`_

Resolve with updated user.

