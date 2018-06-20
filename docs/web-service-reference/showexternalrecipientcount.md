---
title: ShowExternalRecipientCount
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ShowExternalRecipientCount
api_type:
- schema
ms.assetid: db28dbcb-d051-4e5c-a9c2-4b8d5149b4e1
description: ShowExternalRecipientCount 要素は、メッセージの宛先を外部の受信者の数を示すメール ヒントを表示するのには、GetMailTips 操作の消費者があるかどうかを示します。
ms.openlocfilehash: 1fd3ceb629689c560dc60afe01f0413602f79a0d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833491"
---
# <a name="showexternalrecipientcount"></a>ShowExternalRecipientCount

**ShowExternalRecipientCount**要素は、メッセージの宛先を外部の受信者の数を示すメール ヒントを表示するのには、 [GetMailTips 操作](getmailtips-operation.md)の消費者があるかどうかを示します。 
  
```XML
<ShowExternalRecipientCount>true | false</ShowExternalRecipientCount>
```

 **ブール型 (Boolean)**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[MailTipsConfiguration (MailTipsServiceConfiguration)](mailtipsconfiguration-mailtipsserviceconfiguration.md) <br/> |メール ヒント サービスのサービスの構成情報が含まれています。  <br/> |
   
## <a name="text-value"></a>テキスト値

この要素のテキスト値は、 [GetMailTips 操作](getmailtips-operation.md)のコンシューマーは、メッセージの宛先とする外部の受信者の数を示すメール ヒントを表示する必要がある場合**は true**です。 [GetMailTips 操作](getmailtips-operation.md)のコンシューマーは、メッセージの宛先を外部の受信者の数を示すメール ヒントを表示する必要はない場合に、値は**false**です。 
  
## <a name="remarks"></a>備考

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



[GetMailTips 操作](getmailtips-operation.md)


- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

