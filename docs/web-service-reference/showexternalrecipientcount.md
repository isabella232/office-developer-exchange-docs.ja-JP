---
title: ShowExternalRecipientCount
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ShowExternalRecipientCount
api_type:
- schema
ms.assetid: db28dbcb-d051-4e5c-a9c2-4b8d5149b4e1
description: ShowExternalRecipientCount 要素は、GetMailTips 操作のコンシューマーが、メッセージの宛先である外部受信者の数を示すメール ヒントを表示する必要があるかどうかを示します。
ms.openlocfilehash: 30615dcb1091dff01cf13679e3e1ed68c8b25af9
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59539101"
---
# <a name="showexternalrecipientcount"></a>ShowExternalRecipientCount

**ShowExternalRecipientCount** 要素は [、GetMailTips](getmailtips-operation.md)操作のコンシューマーが、メッセージの宛先である外部受信者の数を示すメール ヒントを表示する必要があるかどうかを示します。 
  
```XML
<ShowExternalRecipientCount>true | false</ShowExternalRecipientCount>
```

 **Boolean**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[MailTipsConfiguration (MailTipsServiceConfiguration)](mailtipsconfiguration-mailtipsserviceconfiguration.md) <br/> |メール ヒント サービスのサービス構成情報が含まれる。  <br/> |
   
## <a name="text-value"></a>テキスト値

[GetMailTips](getmailtips-operation.md)操作のコンシューマーが、メッセージの宛先である外部受信者の数を示すメール ヒントを表示する必要がある場合、この要素のテキスト値は true です。 [GetMailTips](getmailtips-operation.md)操作のコンシューマーが、メッセージの宛先である外部受信者の数を示すメール ヒントを表示する必要がない場合、値は false です。  
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



[GetMailTips 操作](getmailtips-operation.md)


- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

