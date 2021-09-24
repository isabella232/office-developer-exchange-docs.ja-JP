---
title: HasIrm
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: fedc04e0-cfd2-4652-a2a8-51de859ae847
description: HasIrm 要素は、会話と現在のフォルダー内の少なくとも 1 つのメッセージが IRM で保護されたメッセージであるかどうかを指定します。
ms.openlocfilehash: ef194c045bfd2b416e382c12381afd68ba56dcf3
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59516693"
---
# <a name="hasirm"></a>HasIrm

**HasIrm 要素は**、会話と現在のフォルダー内の少なくとも 1 つのメッセージが IRM で保護されたメッセージであるかどうかを指定します。 
  
```XML
<HasIrm> true | false </HasIrm>
```

 **Boolean**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[Conversation (ConversationType)](conversation-conversationtype.md)
  
## <a name="text-value"></a>テキスト値

HasIrm 要素の **テキスト値** は、会話内のメッセージが少なくとも 1 つ、現在のフォルダーに IRM がある場合は true です。 それ以外の場合、値は **false です**。
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 Service Pack 1 (SP1) で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |正解  <br/> |
   
## <a name="see-also"></a>関連項目



[Conversation (ConversationType)](conversation-conversationtype.md)


- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

