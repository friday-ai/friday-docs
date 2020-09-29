**friday-server**

> [README](../README.md) / [Globals](../globals.md) / system

# Module: system

## Index

### Classes

* [System](../classes/system.system-1.md)

### Functions

* [getVersion](system.md#getversion)
* [init](system.md#init)
* [saveVersion](system.md#saveversion)
* [shutdown](system.md#shutdown)
* [start](system.md#start)

## Functions

### getVersion

▸ **getVersion**(`this`: [System](../classes/system.system-1.md)): Promise\<Array\<String>>

*Defined in [src/core/system/system.getVersion.ts:10](https://github.com/friday-ai/friday/blob/cd1d9b5/server/src/core/system/system.getVersion.ts#L10)*

Get actual version and last saved version of Friday

#### Parameters:

Name | Type |
------ | ------ |
`this` | [System](../classes/system.system-1.md) |

**Returns:** Promise\<Array\<String>>

Resolve with an array

___

### init

▸ **init**(`this`: [System](../classes/system.system-1.md)): Promise\<void>

*Defined in [src/core/system/system.init.ts:10](https://github.com/friday-ai/friday/blob/cd1d9b5/server/src/core/system/system.init.ts#L10)*

Function to create necessary elements in database at first run of Friday system

#### Parameters:

Name | Type |
------ | ------ |
`this` | [System](../classes/system.system-1.md) |

**Returns:** Promise\<void>

___

### saveVersion

▸ **saveVersion**(`this`: [System](../classes/system.system-1.md), `version`: string): Promise\<[VariableType](../interfaces/variable.variabletype.md)>

*Defined in [src/core/system/system.saveVersion.ts:10](https://github.com/friday-ai/friday/blob/cd1d9b5/server/src/core/system/system.saveVersion.ts#L10)*

Saves actual version of friday

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`this` | [System](../classes/system.system-1.md) | - |
`version` | string | The version to save |

**Returns:** Promise\<[VariableType](../interfaces/variable.variabletype.md)>

Resolve with updated variable

___

### shutdown

▸ **shutdown**(`this`: [System](../classes/system.system-1.md)): Promise\<void>

*Defined in [src/core/system/system.shutdown.ts:7](https://github.com/friday-ai/friday/blob/cd1d9b5/server/src/core/system/system.shutdown.ts#L7)*

Shutdown function fo Friday system

#### Parameters:

Name | Type |
------ | ------ |
`this` | [System](../classes/system.system-1.md) |

**Returns:** Promise\<void>

___

### start

▸ **start**(`this`: [System](../classes/system.system-1.md)): Promise\<void>

*Defined in [src/core/system/system.start.ts:11](https://github.com/friday-ai/friday/blob/cd1d9b5/server/src/core/system/system.start.ts#L11)*

Start function fo Friday system

#### Parameters:

Name | Type |
------ | ------ |
`this` | [System](../classes/system.system-1.md) |

**Returns:** Promise\<void>
