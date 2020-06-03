---
title: ConvertId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConvertId
api_type:
- schema
ms.assetid: 9684c22c-29d4-4f7f-befc-8cd41da56d38
description: 変換 Tid 要素は、サポートされている Exchange 形式間でアイテムとフォルダーの識別子を変換する要求を定義します。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。
ms.openlocfilehash: d421baf1f29fb59a8c6eb2b09e1fa0e8a38ffaa4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44452539"
---
# <a name="convertid"></a>ConvertId

変換**tid**要素は、サポートされている Exchange 形式間でアイテムとフォルダーの識別子を変換する要求を定義します。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。 
  
```xml
<ConvertId DestinationFormat="">
   <SourceIds/>
</ConvertId>
```

 **ConvertIdType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**DestinationFormat** <br/> |変換されたすべての識別子に対して返される識別子の形式を記述します。 DestinationFormat は、IdFormatType によって記述されます。  <br/> |
   
#### <a name="destinationformat-attribute"></a>DestinationFormat 属性

|**値**|**説明**|
|:-----|:-----|
|**EwsLegacyId** <br/> |Exchange 2007 の最初のリリースバージョンで提供される Exchange Web サービス識別子に使用される識別子の形式を表します。  <br/> |
|**EwsId** <br/> |Exchange Server 2007 SP1 以降の Exchange Web サービス識別子に使用される識別子の形式を表します。  <br/> |
|**EntryId** <br/> |PR_ENTRYID プロパティのように、MAPI 識別子を表します。  <br/> |
|**HexEntryId** <br/> |可用性カレンダーイベント識別子を表します。 これは、PR_ENTRYID プロパティを16進数でエンコードした表記です。  <br/> |
|**StoreId** <br/> |Exchange ストア識別子を表します。  <br/> |
|**OwaId** <br/> |Outlook Web Access 識別子の形式を表します。  <br/> |
   
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[SourceIds](sourceids.md) <br/> |変換するソース識別子を含みます。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



[ConvertId 操作](convertid-operation.md)


- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)


[識別子の変換](https://msdn.microsoft.com/library/a5391746-b6ef-4f48-8fc8-8255258651aa%28Office.15%29.aspx)

