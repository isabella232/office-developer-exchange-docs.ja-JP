---
title: ConvertId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ConvertId
api_type:
- schema
ms.assetid: 9684c22c-29d4-4f7f-befc-8cd41da56d38
description: ConvertId 要素は、サポートされているファイル形式間でアイテム識別子とフォルダー識別子を変換する要求Exchangeします。 この要素は、2007 Microsoft Exchange Server パック 1 (SP1) で導入されました。
ms.openlocfilehash: fe7d46697ba72ba6458136541488f5cd498169f4
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59545560"
---
# <a name="convertid"></a>ConvertId

**ConvertId 要素は**、サポートされているファイル形式間でアイテム識別子とフォルダー識別子を変換Exchangeします。 この要素は、2007 Microsoft Exchange Server パック 1 (SP1) で導入されました。 
  
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
|**DestinationFormat** <br/> |変換された識別子すべてについて返される識別子の形式を説明します。 DestinationFormat は IdFormatType で説明します。  <br/> |
   
#### <a name="destinationformat-attribute"></a>DestinationFormat 属性

|**値**|**説明**|
|:-----|:-----|
|**EwsLegacyId** <br/> |2007 年の初期リリース バージョンで提供Exchange Web サービス識別子に使用される識別子の形式Exchangeします。  <br/> |
|**EwsId** <br/> |2007 SP1 で始まる Web サービスExchangeに使用される識別子の形式Exchange Serverします。  <br/> |
|**EntryId** <br/> |MAPI 識別子を表します。このプロパティPR_ENTRYIDします。  <br/> |
|**HexEntryId** <br/> |利用可能な予定表のイベント識別子を表します。 これは、16 進数でエンコードされたプロパティのPR_ENTRYIDです。  <br/> |
|**StoreId** <br/> |ストア識別子のExchangeを表します。  <br/> |
|**OwaId** <br/> |Web Access 識別子Outlook形式を表します。  <br/> |
   
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[SourceIds](sourceids.md) <br/> |変換するソース識別子が含まれる。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



[ConvertId 操作](convertid-operation.md)


- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)


[識別子の変換](https://msdn.microsoft.com/library/a5391746-b6ef-4f48-8fc8-8255258651aa%28Office.15%29.aspx)

