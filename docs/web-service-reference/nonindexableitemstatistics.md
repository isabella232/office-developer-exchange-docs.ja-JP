---
title: NonIndexableItemStatistics
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 12f2934a-008c-4236-b8b3-7c7b6b5707e2
description: NonIndexableItemStatistics 要素には、インデックスを作成できなかったアイテムの統計の配列が含まれています。
ms.openlocfilehash: 5a11bd4d7ef0c574f26580613063a885530176f9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466732"
---
# <a name="nonindexableitemstatistics"></a>NonIndexableItemStatistics

**Nonindexableitemstatistics**要素には、インデックスを作成できなかったアイテムの統計の配列が含まれています。 
  
```XML
<NonIndexableItemStatistics>
   <NonIndexableItemStatistic/>
</NonIndexableItemStatistics>
```

 **ArrayOfNonIndexableItemStatisticsType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

[NonIndexableItemStatistic](nonindexableitemstatistic.md)
  
### <a name="parent-elements"></a>親要素

[GetNonIndexableItemStatisticsResponse](getnonindexableitemstatisticsresponse.md) 、 [GetNonIndexableItemStatisticsResponseMessage](getnonindexableitemstatisticsresponsemessage.md)
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空にすることができます。  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



[GetNonIndexableItemStatistics 操作](getnonindexableitemstatistics-operation.md)


- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

