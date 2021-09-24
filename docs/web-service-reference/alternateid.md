---
title: AlternateId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- AlternateId
api_type:
- schema
ms.assetid: 9c01fdc3-4adf-4e23-bc33-45d2a45ea08b
description: AlternateId 要素は、要求で変換する識別子と、応答内の変換された識別子の結果を表します。
ms.openlocfilehash: 6346a45b48eb811cac705d8da85dc77e6c18262c
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59520942"
---
# <a name="alternateid"></a>AlternateId

**AlternateId 要素** は、要求で変換する識別子と、応答内の変換された識別子の結果を表します。 
  
```XML
<AlternateId Id="" Format="" Mailbox="" IsArchive=""/>
```

 **AlternateIdType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|ID  <br/> |ConvertId 操作要求のソース識別子を説明し [、ConvertId](convertid-operation.md) 操作応答の宛先識別子 [を記述](convertid-operation.md) します。  <br/> |
|フォーマット  <br/> |[ConvertId](convertid-operation.md)操作要求のソース形式を説明し、変換先の形式を ConvertId 操作応答[で記述](convertid-operation.md)します。 変換先の形式は、 **要求内の ConvertId** 要素の [DestinationFormat](convertid.md) 属性によって記述されます。 この属性の種類は **IdFormatType です**。  <br/> |
|Mailbox  <br/> |変換する識別子を含むメールボックスのプライマリ簡易メール転送プロトコル (SMTP) アドレスについて説明します。  <br/> |
|IsArchive  <br/> |識別子がアーカイブ済みアイテムまたはフォルダーを表すかどうかを示します。 true の値 **は** 、識別子がアーカイブされたアイテムまたはフォルダーを表します。 この属性は省略可能です。  <br/> |
   
#### <a name="format-attribute-values"></a>属性値の書式設定

|**値**|**説明**|
|:-----|:-----|
|EwsLegacyId  <br/> |2007 年の初期リリース バージョンExchange Web サービスによって生成される識別子Exchangeします。  <br/> |
|EwsId  <br/> |2007 SP1 から始まる Web サービスExchange生成されるExchange説明します。  <br/> |
|EntryId  <br/> |MAPI 識別子について説明します。このプロパティ **PR_ENTRYIDします。**  <br/> |
|HexEntryId  <br/> |プロパティの 16 進数でエンコードされた **表現PR_ENTRYID** します。 これは、利用可能な予定表のイベント識別子の形式です。  <br/> |
|StoreId  <br/> |ストアExchangeについて説明します。  <br/> |
|OwaId  <br/> |識別子をOutlook Web Appします。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ConvertIdResponseMessage](convertidresponsemessage.md) <br/> |ConvertId 操作要求の状態と結果 [を格納](convertid-operation.md) します。  <br/> |
|[SourceIds](sourceids.md) <br/> |変換するソース識別子が含まれる。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>注釈

**AlternateId 要素は**[、ConvertId](convertid-operation.md)操作要求で変換されるソース識別子と [ConvertIdResponse](convertidresponse.md)要素の変換された識別子の 2 つの識別子を表します。 
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

||||
|:-----|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目

- [ConvertId 操作](convertid-operation.md)
- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)
- [識別子の変換](https://msdn.microsoft.com/library/a5391746-b6ef-4f48-8fc8-8255258651aa%28Office.15%29.aspx)

