# house

> [**friday-server**](./)

[Globals](https://github.com/friday-ai/friday-docs/tree/7469fd0637aa28a674d6c68645188ee863701e30/node-js-api-1/globals.md) / [house](house.md) /

## External module: house

#### Index

**Classes**

* [House](https://github.com/friday-ai/friday-docs/tree/7469fd0637aa28a674d6c68645188ee863701e30/node-js-api-1/classes/house.house-1.md)

**Interfaces**

* [HouseType](https://github.com/friday-ai/friday-docs/tree/7469fd0637aa28a674d6c68645188ee863701e30/node-js-api-1/interfaces/house.housetype.md)

**Functions**

* [create](house.md#create)
* [destroy](house.md#destroy)
* [getAll](house.md#getall)
* [getById](house.md#getbyid)
* [update](house.md#update)

### Functions

#### create

▸ **create**\(`house`: [HouseType](https://github.com/friday-ai/friday-docs/tree/7469fd0637aa28a674d6c68645188ee863701e30/node-js-api-1/interfaces/house.housetype.md)\): _`Promise<HouseType>`_

Defined in house/house.create.ts:20

Create an house.

**`example`**

```text
friday.house.create({
   id: '7774f404-1947-4908-b2a4-5ab5df808693',
   name: 'Sample House',
   latitude: '34.0012295',
   longitude: '-118.8067245'
});
```

**Parameters:**

| Name | Type | Description |
| :--- | :--- | :--- |
| `house` | [HouseType](https://github.com/friday-ai/friday-docs/tree/7469fd0637aa28a674d6c68645188ee863701e30/node-js-api-1/interfaces/house.housetype.md) | An house object. |

**Returns:** _`Promise<HouseType>`_

Resolve with created house.

#### destroy

▸ **destroy**\(`id`: string\): _`Promise<void>`_

Defined in house/house.destroy.ts:14

Destroy an house.

**`example`**

```text
friday.house.destroy('d5988c5b-c3ae-4aff-ab63-037d855c1978');
```

**Parameters:**

| Name | Type | Description |
| :--- | :--- | :--- |
| `id` | string | Id of house. |

**Returns:** _`Promise<void>`_

#### getAll

▸ **getAll**\(`options?`: `GetOptions`\): _`Promise<HouseType[]>`_

Defined in house/house.getAll.ts:26

Get all houses.

**`example`**

```text
friday.house.getAll({
   scope: '',
   take: 20,
   skip: 0
 });
```

**Parameters:**

| Name | Type | Description |
| :--- | :--- | :--- |
| `options?` | `GetOptions` | Options of the query. |

**Returns:** _`Promise<HouseType[]>`_

Resolve with house array.

#### getById

▸ **getById**\(`id`: string, `scope?`: undefined \| string\): _`Promise<HouseType>`_

Defined in house/house.getById.ts:16

Get a house by id.

**`example`**

```text
friday.device.getById('6be1d66d-da22-47c2-b7d0-54b51429db62', 'full');
```

**Parameters:**

| Name | Type | Description |
| :--- | :--- | :--- |
| `id` | string | Id of house. |
| `scope?` | undefined \| string | Scope option. \(Optional\) |

**Returns:** _`Promise<HouseType>`_

Resolve with house.

#### update

▸ **update**\(`house`: [HouseType](https://github.com/friday-ai/friday-docs/tree/7469fd0637aa28a674d6c68645188ee863701e30/node-js-api-1/interfaces/house.housetype.md)\): _`Promise<HouseType>`_

Defined in house/house.update.ts:18

Update an house.

**`example`**

```text
friday.house.update({
  id: '40d43cf1-2127-41e9-ac69-9e39636fac20'
  name: 'house update'
});
```

**Parameters:**

| Name | Type | Description |
| :--- | :--- | :--- |
| `house` | [HouseType](https://github.com/friday-ai/friday-docs/tree/7469fd0637aa28a674d6c68645188ee863701e30/node-js-api-1/interfaces/house.housetype.md) | An house object. |

**Returns:** _`Promise<HouseType>`_

Resolve with updated house.

