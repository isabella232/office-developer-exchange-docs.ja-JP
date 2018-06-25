---
title: FlaggedForAction
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FlaggedForAction
api_type:
- schema
ms.assetid: 6a08c48a-7b32-4754-8940-adbda55e8133
description: FlaggedForAction 要素を適用する場合の条件または例外の順序で受信したメッセージに表示する必要がありますアクションの値のフラグを指定します。
ms.openlocfilehash: 5b6e714512edcf12ded2c04f414d047b8622d305
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760555"
---
# <a name="flaggedforaction"></a>FlaggedForAction

**FlaggedForAction**要素を適用する場合の条件または例外の順序で受信したメッセージに表示する必要がありますアクションの値のフラグを指定します。 
  
```XML
<FlaggedForAction/>
```

 **FlaggedForActionType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[条件](conditions.md) <br/> |条件を表しますが、満たされるとときに、ルールのルールの処理をトリガーします。  <br/> |
|[Exceptions](exceptions.md) <br/> |受信トレイ ルールの使用可能なルールの例外条件をすべてを表す例外を表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は必須です。 この要素の使用可能なテキスト値は、次のように。
  
- Any
    
- Call
    
- DoNotForward
    
- FollowUp
    
- FYI
    
- Forward
    
- NoResponseNecessary
    
- Read
    
- Reply
    
- ReplyToAll
    
- Review
    
## <a name="remarks"></a>備考

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |True  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

