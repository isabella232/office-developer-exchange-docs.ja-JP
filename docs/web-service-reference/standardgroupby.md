---
title: StandardGroupBy
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- StandardGroupBy
api_type:
- schema
ms.assetid: 04a84f71-b7eb-44dc-ac2c-ed504b52c463
description: StandardGroupBy 要素は、グループ化された FindItem 操作の標準のグループ化および集約メカニズムを表します。
ms.openlocfilehash: 3e135feba322979de3d66d5a45d423654ccc9100
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467558"
---
# <a name="standardgroupby"></a>StandardGroupBy

**Standardgroupby**要素は、グループ化された FindItem 操作の標準のグループ化および集約メカニズムを表します。 
  
[FindItem](finditem.md)
  
[DistinguishedGroupBy](distinguishedgroupby.md)
  
[StandardGroupBy](standardgroupby.md)
  
```xml
<StandardGroupBy/>
```

 **StandardGroupByType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[DistinguishedGroupBy](distinguishedgroupby.md) <br/> |FindItem クエリの標準的なグループを提供します。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は必須です。 この要素に使用できる値は**ConversationTopic**のみです。 **ConversationTopic**によってグループ化されたメッセージ: ConversationTopic およびアイテムの集計: DateTimeReceived (最大)。 集計の詳細については、「 [AggregateOn](aggregateon.md)」を参照してください。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目




  [FindItem 操作](finditem-operation.md)
  
[FindItem](finditem.md)


[アイテムの検索](https://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

