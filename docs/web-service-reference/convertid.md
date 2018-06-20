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
description: ConvertId 要素は、Exchange でサポートされる形式の間でのアイテムおよびフォルダーの識別子を変換するための要求を定義します。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。
ms.openlocfilehash: 956f6464fd9013f9e72d2915f21c3b011d0add5b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759767"
---
# <a name="convertid"></a>ConvertId

**ConvertId**要素は、Exchange でサポートされる形式の間でのアイテムおよびフォルダーの識別子を変換するための要求を定義します。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。 
  
```xml
<ConvertId DestinationFormat="">
   <SourceIds/>
</ConvertId>
```

 **ConvertIdType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**DestinationFormat** <br/> |変換後のすべての識別子の返される識別子の形式を表します。 DestinationFormat は、IdFormatType で説明されています。  <br/> |
   
#### <a name="destinationformat-attribute"></a>DestinationFormat 属性

|**値**|**説明**|
|:-----|:-----|
|**EwsLegacyId** <br/> |初期リリース版の Exchange 2007 で提供されている Exchange Web サービスの識別子に使用される識別子の形式を表します。  <br/> |
|**EwsId** <br/> |Exchange Web サービスの識別子が Exchange Server 2007 sp1 の起動に使用される識別子の形式を表します。  <br/> |
|**エントリ Id** <br/> |PR_ENTRYID プロパティと同様に、MAPI id を表します。  <br/> |
|**HexEntryId** <br/> |可用性の予定表のイベント識別子を表します。 これは、PR_ENTRYID プロパティの 16 進数でエンコードされた表現です。  <br/> |
|**StoreId** <br/> |Exchange ストアの id を表します。  <br/> |
|**OwaId** <br/> |Outlook Web Access の識別子の形式を表します。  <br/> |
   
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[SourceIds](sourceids.md) <br/> |変換するソース識別子が含まれます。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="remarks"></a>備考

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



[ConvertId 操作](convertid-operation.md)


- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)


[識別子に変換します。](http://msdn.microsoft.com/library/a5391746-b6ef-4f48-8fc8-8255258651aa%28Office.15%29.aspx)

