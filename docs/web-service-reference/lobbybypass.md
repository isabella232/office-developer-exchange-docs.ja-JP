---
title: LobbyBypass
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: e05ed6eb-00ae-49c8-8341-43f6e0d728ff
description: LobbyBypass 要素は、オンライン会議、仮想ロビーをバイパスする設定を指定します。
ms.openlocfilehash: 9ecc920acd9e1aea3476ad1194d6c7d0529b21c7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832246"
---
# <a name="lobbybypass"></a>LobbyBypass

**LobbyBypass**要素は、オンライン会議、仮想ロビーをバイパスする設定を指定します。 
  
```XML
<LobbyBypass> Disabled | EnabledForGatewayParticipants </LobbyBypass>
```

 **LobbyBypassType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[OnlineMeetingSettings](onlinemeetingsettings.md)
  
## <a name="text-value"></a>テキスト値

**LobbyBypass**要素のテキスト値には、**無効**または**EnabledForGatewayParticipants**のいずれかを指定できます。 **無効になっている**値は、仮想ロビーをすべての会議出席者がアクセスする必要がありますので、ロビーのバイパスが無効になっていることを示します。 **EnabledForGatewayParticipants**値では、参加者の電話でロビーのバイパスが有効であることを示します。 
  
## <a name="remarks"></a>備考

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  

