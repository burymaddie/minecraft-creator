---
# DO NOT TOUCH — This file was automatically generated. See https://github.com/mojang/minecraftapidocsgenerator to modify descriptions, examples, etc.
author: jakeshirley
ms.author: jashir
ms.service: minecraft-bedrock-edition
title: minecraft/server.GameRuleChangeAfterEventSignal Class
description: Contents of the @minecraft/server.GameRuleChangeAfterEventSignal class.
monikerRange: "=minecraft-bedrock-experimental"
---
# GameRuleChangeAfterEventSignal Class

> [!CAUTION]
> This class is still in pre-release.  Its signature may change or it may be removed in future releases.

Manages callbacks that are connected to when a world.gameRules property has changed.

## Methods
- [subscribe](#subscribe)
- [unsubscribe](#unsubscribe)

### **subscribe**
`
subscribe(callback: (arg: GameRuleChangeAfterEvent) => void): (arg: GameRuleChangeAfterEvent) => void
`

Adds a callback that will be called when a world.gameRules property is changed.

#### **Parameters**
- **callback**: (arg: [*GameRuleChangeAfterEvent*](GameRuleChangeAfterEvent.md)) => *void*

#### **Returns** (arg: [*GameRuleChangeAfterEvent*](GameRuleChangeAfterEvent.md)) => *void*

> [!IMPORTANT]
> This function can't be called in read-only mode.

### **unsubscribe**
`
unsubscribe(callback: (arg: GameRuleChangeAfterEvent) => void): void
`

Removes a callback from being called when a world.gameRules property is changed.

#### **Parameters**
- **callback**: (arg: [*GameRuleChangeAfterEvent*](GameRuleChangeAfterEvent.md)) => *void*

> [!IMPORTANT]
> This function can't be called in read-only mode.

> [!WARNING]
> This function can throw errors.
