**friday-server**

> [README](../README.md) / [Globals](../globals.md) / plugin

# Module: plugin

## Index

### Classes

* [Plugin](../classes/plugin.plugin-1.md)

### Interfaces

* [PluginType](../interfaces/plugin.plugintype.md)

### Functions

* [create](plugin.md#create)
* [destroy](plugin.md#destroy)
* [getAll](plugin.md#getall)
* [getById](plugin.md#getbyid)
* [update](plugin.md#update)

## Functions

### create

▸ **create**(`plugin`: [PluginType](../interfaces/plugin.plugintype.md)): Promise\<[PluginType](../interfaces/plugin.plugintype.md)>

*Defined in [src/core/plugin/plugin.create.ts:23](https://github.com/friday-ai/friday/blob/cd1d9b5/server/src/core/plugin/plugin.create.ts#L23)*

Create a plugin.

**`example`** 
````
friday.plugin.create({
   id: '3ee32844-dad1-4d4d-9b2d-fe5f7766854c',
   name: 'Sample plugin',
   version: '1.0.0',
   url: 'sample url',
   enabled: true,
   satelliteId: '384f3c02-0eec-4497-8a83-c900f1df4db5'
});
````

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`plugin` | [PluginType](../interfaces/plugin.plugintype.md) | A plugin object. |

**Returns:** Promise\<[PluginType](../interfaces/plugin.plugintype.md)>

Resolve with created plugin.

___

### destroy

▸ **destroy**(`id`: string): Promise\<void>

*Defined in [src/core/plugin/plugin.destroy.ts:13](https://github.com/friday-ai/friday/blob/cd1d9b5/server/src/core/plugin/plugin.destroy.ts#L13)*

Destroy a plugin.

**`example`** 
````
friday.plugin.destroy('833e9fe3-f753-4b2e-8949-ca4684e4f886');
````

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`id` | string | Id of plugin. |

**Returns:** Promise\<void>

___

### getAll

▸ **getAll**(`options?`: GetOptions): Promise\<[PluginType](../interfaces/plugin.plugintype.md)[]>

*Defined in [src/core/plugin/plugin.getAll.ts:25](https://github.com/friday-ai/friday/blob/cd1d9b5/server/src/core/plugin/plugin.getAll.ts#L25)*

Get all plugins.

**`example`** 
````
friday.plugin.getAll({
   scope: '',
   take: 20,
   skip: 0
 });
````

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`options?` | GetOptions | Options of the query. |

**Returns:** Promise\<[PluginType](../interfaces/plugin.plugintype.md)[]>

Resolve with plugin array.

___

### getById

▸ **getById**(`id`: string, `scope?`: undefined \| string): Promise\<[PluginType](../interfaces/plugin.plugintype.md)>

*Defined in [src/core/plugin/plugin.getById.ts:15](https://github.com/friday-ai/friday/blob/cd1d9b5/server/src/core/plugin/plugin.getById.ts#L15)*

Get a plugin by id.

**`example`** 
````
friday.plugin.getById('8d77999c-4b4f-447d-9fb3-851985981f1e', 'full');
````

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`id` | string | Id of plugin. |
`scope?` | undefined \| string | Scope option. (Optional) |

**Returns:** Promise\<[PluginType](../interfaces/plugin.plugintype.md)>

Resolve with plugin.

___

### update

▸ **update**(`id`: string, `plugin`: [PluginType](../interfaces/plugin.plugintype.md)): Promise\<[PluginType](../interfaces/plugin.plugintype.md)>

*Defined in [src/core/plugin/plugin.update.ts:20](https://github.com/friday-ai/friday/blob/cd1d9b5/server/src/core/plugin/plugin.update.ts#L20)*

Update a plugin.

**`example`** 
````
friday.plugin.update(
'40d43cf1-2127-41e9-ac69-9e39636fac20',
{
  id: '40d43cf1-2127-41e9-ac69-9e39636fac20'
  name: 'plugin update'
});
````

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`id` | string | Id of plugin |
`plugin` | [PluginType](../interfaces/plugin.plugintype.md) | A plugin object. |

**Returns:** Promise\<[PluginType](../interfaces/plugin.plugintype.md)>

Resolve with updated plugin.
