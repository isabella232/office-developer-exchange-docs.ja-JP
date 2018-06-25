---
title: HasIrm
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: fedc04e0-cfd2-4652-a2a8-51de859ae847
description: HasIrm 要素は、会話と現在のフォルダー内の 1 つ以上のメッセージが IRM で保護されたメッセージかどうかを指定します。
ms.openlocfilehash: c129370d7920da7cf1f9f32eed2f075e6c21cf8b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19831803"
---
# <a name="hasirm"></a>HasIrm

**HasIrm**要素は、会話と現在のフォルダー内の 1 つ以上のメッセージが IRM で保護されたメッセージかどうかを指定します。 
  
```XML
<HasIrm> true | false </HasIrm>
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

**会話し、現在のフォルダー内の 1 つ以上のメッセージが IRM を持つ場合、 **HasIrm**要素のテキスト値は** それ以外の場合、値が**false**にします。
  
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

