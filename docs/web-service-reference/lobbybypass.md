---
title: LobbyBypass
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: e05ed6eb-00ae-49c8-8341-43f6e0d728ff
description: LobbyBypass 要素は、仮想ロビーをバイパスするオンライン会議の設定を指定します。
ms.openlocfilehash: 6940428c944b9d4d64acc6dbbf3993576e1932eb
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458097"
---
# <a name="lobbybypass"></a>LobbyBypass

**Lobbybypass**要素は、仮想ロビーをバイパスするオンライン会議の設定を指定します。 
  
```XML
<LobbyBypass> Disabled | EnabledForGatewayParticipants </LobbyBypass>
```

 **LobbyBypassType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[OnlineMeetingSettings](onlinemeetingsettings.md)
  
## <a name="text-value"></a>テキスト値

**Lobbybypass**要素のテキスト値は、Disabled または**EnabledForGatewayParticipants**のいずれか**に**なります。 **Disabled**値は、すべての会議の出席者が仮想ロビーを介してアクセスする必要があるように、ロビーバイパスが無効になっていることを示します。 **EnabledForGatewayParticipants**の値は、電話の参加者に対してロビーバイパスが有効になっていることを示します。 
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  

