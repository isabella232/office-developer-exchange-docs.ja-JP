---
title: AlternateId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AlternateId
api_type:
- schema
ms.assetid: 9c01fdc3-4adf-4e23-bc33-45d2a45ea08b
description: AlternateId 要素は、要求で変換する識別子と、応答で変換された id の結果を示します。
ms.openlocfilehash: 26df68bd814c2d323630c6bb40b4c31745017c71
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527454"
---
# <a name="alternateid"></a>AlternateId

**Alternateid**要素は、要求で変換する識別子と、応答で変換された id の結果を示します。 
  
```XML
<AlternateId Id="" Format="" Mailbox="" IsArchive=""/>
```

 **AlternateIdType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|ID  <br/> |変換[tid 操作](convertid-operation.md)要求のソース識別子を記述し、変換[tid 操作](convertid-operation.md)応答で宛先識別子を記述します。  <br/> |
|Format  <br/> |変換[tid 操作](convertid-operation.md)要求のソース形式を記述し、変換[tid 操作](convertid-operation.md)の応答で宛先の形式を記述します。 転送先の形式は、要求の変換[tid](convertid.md)要素の**destinationformat**属性によって記述されます。 この属性の型は**IdFormatType**です。  <br/> |
|メールボックス  <br/> |変換する識別子を含むメールボックスのプライマリ SMTP (Simple Mail Transfer Protocol) アドレスについて説明します。  <br/> |
|IsArchive  <br/> |識別子がアーカイブされたアイテムまたはフォルダーを表しているかどうかを示します。 値が**true の場合**は、識別子がアーカイブされたアイテムまたはフォルダーを表していることを示します。 この属性は省略可能です。  <br/> |
   
#### <a name="format-attribute-values"></a>書式属性値

|**値**|**説明**|
|:-----|:-----|
|EwsLegacyId  <br/> |Exchange 2007 の最初のリリースバージョンで Exchange Web サービスによって生成された識別子について説明します。  <br/> |
|EwsId  <br/> |Exchange 2007 SP1 以降の Exchange Web サービスによって生成される識別子について説明します。  <br/> |
|EntryId  <br/> |**PR_ENTRYID**プロパティのように、MAPI 識別子について説明します。  <br/> |
|HexEntryId  <br/> |**PR_ENTRYID**プロパティの16進数でエンコードされた表現を記述します。 これは、可用性カレンダーイベント識別子の形式です。  <br/> |
|StoreId  <br/> |Exchange ストア識別子について説明します。  <br/> |
|OwaId  <br/> |Outlook Web App 識別子を表します。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ConvertIdResponseMessage](convertidresponsemessage.md) <br/> |[状態]-[バケット][操作](convertid-operation.md)要求の状態と結果を格納します。  <br/> |
|[SourceIds](sourceids.md) <br/> |変換するソース識別子を含みます。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>注釈

**Alternateid**要素[は、2](convertid-operation.md)つの識別子、変換される変換元識別子、および[ConvertIdResponse](convertidresponse.md)要素の変換された識別子を表します。 
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

||||
|:-----|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |メッセージスキーマ  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目

- [ConvertId 操作](convertid-operation.md)
- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)
- [識別子の変換](https://msdn.microsoft.com/library/a5391746-b6ef-4f48-8fc8-8255258651aa%28Office.15%29.aspx)

