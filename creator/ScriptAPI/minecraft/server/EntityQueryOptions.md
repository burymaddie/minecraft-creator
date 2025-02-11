---
# DO NOT TOUCH — This file was automatically generated. See https://github.com/mojang/minecraftapidocsgenerator to modify descriptions, examples, etc.
author: jakeshirley
ms.author: jashir
ms.service: minecraft-bedrock-edition
title: minecraft/server.EntityQueryOptions Interface
description: Contents of the @minecraft/server.EntityQueryOptions class.
---
# EntityQueryOptions Interface

Contains options for selecting entities within an area.

## Properties

### **closest**
`closest?: number;`

Limits the number of entities to return, opting for the closest N entities as specified by this property. The location value must also be specified on the query options object.

Type: *number*

### **excludeFamilies**
`excludeFamilies?: string[];`

Excludes entities that match one or more of the specified families.

Type: *string*[]

### **excludeGameModes**
`excludeGameModes?: GameMode[];`

Excludes entities if have a specific gamemode that matches the specified gamemode.

Type: [*GameMode*](GameMode.md)[]

### **excludeNames**
`excludeNames?: string[];`

Excludes entities that have a name that match one of the specified values.

Type: *string*[]

### **excludeTags**
`excludeTags?: string[];`

Excludes entities with a tag that matches one of the specified values.

Type: *string*[]

### **excludeTypes**
`excludeTypes?: string[];`

Excludes entities if they are one of the specified types.

Type: *string*[]

### **families**
`families?: string[];`

If specified, includes entities that match all of the specified families.

Type: *string*[]

### **farthest**
`farthest?: number;`

Limits the number of entities to return, opting for the farthest N entities as specified by this property. The location value must also be specified on the query options object.

Type: *number*

### **gameMode**
`gameMode?: GameMode;`

If specified, includes entities with a gamemode that matches the specified gamemode.

Type: [*GameMode*](GameMode.md)

### **location**
`location?: Vector3;`

Adds a seed location to the query that is used in conjunction with closest, farthest, limit, volume, and distance properties.

Type: [*Vector3*](Vector3.md)

### **maxDistance**
`maxDistance?: number;`

If specified, includes entities that are less than this distance away from the location specified in the location property.

Type: *number*

### **maxHorizontalRotation**
`maxHorizontalRotation?: number;`

If specified, will only include entities that have at most this horizontal rotation.

Type: *number*

### **maxLevel**
`maxLevel?: number;`

If defined, only players that have at most this level are returned.

Type: *number*

### **maxVerticalRotation**
`maxVerticalRotation?: number;`

If specified, only entities that have at most this vertical rotation are returned.

Type: *number*

### **minDistance**
`minDistance?: number;`

If specified, includes entities that are least this distance away from the location specified in the location property.

Type: *number*

### **minHorizontalRotation**
`minHorizontalRotation?: number;`

If specified, will only include entities that have at a minimum this horizontal rotation.

Type: *number*

### **minLevel**
`minLevel?: number;`

If defined, only players that have at least this level are returned.

Type: *number*

### **minVerticalRotation**
`minVerticalRotation?: number;`

If specified, will only include entities that have at least this vertical rotation.

Type: *number*

### **name**
`name?: string;`

Includes entities with the specified name.

Type: *string*

### **scoreOptions**
`scoreOptions?: EntityQueryScoreOptions[];`

Gets/sets a collection of EntityQueryScoreOptions objects with filters for specific scoreboard objectives.

Type: [*EntityQueryScoreOptions*](EntityQueryScoreOptions.md)[]

### **tags**
`tags?: string[];`

Includes entities that match all of the specified tags.

Type: *string*[]

### **type**
`type?: string;`

If defined, entities that match this type are included.

Type: *string*

::: moniker range="=minecraft-bedrock-experimental"
### **volume**
`volume?: BlockAreaSize;`

In conjunction with location, specified a cuboid volume of entities to include.

Type: [*BlockAreaSize*](BlockAreaSize.md)

> [!CAUTION]
> This property is still in pre-release.  Its signature may change or it may be removed in future releases.
::: moniker-end
