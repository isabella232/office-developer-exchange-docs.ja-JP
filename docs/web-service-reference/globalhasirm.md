---
title: GlobalHasIrm
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 425272b2-7a4e-4376-aea9-d9b10c1ad6ee
description: GlobalHasIrm 要素は、会話ではすべてのフォルダーの 1 つ以上のメッセージは、IRM で保護されたメッセージかどうかを指定します。
ms.openlocfilehash: ad3eafcb38829e7ea57cbc7535b0f5411ad595d2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19831717"
---
# <a name="globalhasirm"></a>GlobalHasIrm

**GlobalHasIrm**要素は、会話ではすべてのフォルダーの 1 つ以上のメッセージは、IRM で保護されたメッセージかどうかを指定します。 
  
```XML
<GlobalHasIrm> true | false </GlobalHasIrm>
```

 **ブール型 (Boolean)**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[会話 (ConversationType)](conversation-conversationtype.md)
  
## <a name="text-value"></a>テキスト値

**会話ではすべてのフォルダーの 1 つ以上のメッセージが IRM で保護されたメッセージの場合、 **GlobalHasIrm**要素のテキスト値は** それ以外の場合、値は、 **false**です。
  
## <a name="remarks"></a>備考

この要素は Exchange Server 2013 Service Pack 1 (SP1) で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |True  <br/> |
   
## <a name="see-also"></a>関連項目



[会話 (ConversationType)](conversation-conversationtype.md)


- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

