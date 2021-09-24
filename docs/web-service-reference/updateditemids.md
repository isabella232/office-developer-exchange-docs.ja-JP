---
title: UpdatedItemIds
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 9199aeb2-abdf-40c5-8743-40b61853c951
description: UpdatedItemIds 要素は、更新されたアラーム アイテムの識別子を指定します。
ms.openlocfilehash: 59e17e32d5df3f8a6000b05899f2fe0c5de2ec00
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59538612"
---
# <a name="updateditemids"></a>UpdatedItemIds

**UpdatedItemIds 要素** は、更新されたアラーム アイテムの識別子を指定します。 
  
```XML
<UpdatedItemIds>
   <ItemId></ItemId>
</UpdatedItemIds>

```

 **NonEmptyArrayOfItemIdsType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

[ItemId](itemid.md)
  
### <a name="parent-elements"></a>親要素

[PerformReminderActionResponse](performreminderactionresponse.md)
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
[PerformReminderAction](performreminderaction-operation.md)操作が正常に完了しなかった場合、またはサーバーで変更が行われた場合 **、UpdatedItemIds** 要素は空の値として返されます。 
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |正解  <br/> |
   
## <a name="see-also"></a>関連項目



[PerformReminderActionResponse](performreminderactionresponse.md)


- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

