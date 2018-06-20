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
description: AlternateId 要素は、要求と応答に変換された識別子の結果に変換するのには識別子について説明します。
ms.openlocfilehash: e4d29087b63b52638dd93e4e3b643cdee39a5b97
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759312"
---
# <a name="alternateid"></a>AlternateId

**AlternateId**要素は、要求と応答に変換された識別子の結果に変換するのには識別子について説明します。 
  
```XML
<AlternateId Id="" Format="" Mailbox="" IsArchive=""/>
```

 **AlternateIdType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|ID  <br/> |[ConvertId 操作](convertid-operation.md)の要求の送信元識別子および[ConvertId 操作](convertid-operation.md)の応答の送信先識別子を説明します。  <br/> |
|Format  <br/> |[ConvertId 操作](convertid-operation.md)の要求のソース フォーマットおよび[ConvertId 操作](convertid-operation.md)の応答に変換先の形式を説明します。 変換先の形式は、要求内の[ConvertId](convertid.md)要素の**DestinationFormat**属性で表されます。 この属性は、型**IdFormatType**のです。  <br/> |
|メールボックス  <br/> |変換するための識別子が含まれているメールボックス プライマリ簡易メール転送プロトコル (SMTP) アドレスについて説明します。  <br/> |
|IsArchive  <br/> |アーカイブされたアイテムまたはフォルダーの識別子を表すかどうかを示します。 **True**の場合は、識別子がアーカイブされたアイテムまたはフォルダーを表すことを示します。 この属性は、省略可能です。  <br/> |
   
#### <a name="format-attribute-values"></a>属性の値を書式設定

|**値**|**説明**|
|:-----|:-----|
|EwsLegacyId  <br/> |Exchange 2007 の最初のリリース版の Exchange Web サービスによって生成される識別子について説明します。  <br/> |
|EwsId  <br/> |Exchange 2007 SP1 以降の Exchange Web サービスによって生成される識別子について説明します。  <br/> |
|EntryId  <br/> |**PR_ENTRYID**プロパティと同様に、MAPI 識別子をについて説明します。  <br/> |
|HexEntryId  <br/> |**PR_ENTRYID**プロパティの 16 進数でエンコードされた表現を説明します。 これは、可用性の予定表のイベント識別子の形式です。  <br/> |
|StoreId  <br/> |Exchange ストア識別子をについて説明します。  <br/> |
|OwaId  <br/> |Outlook Web App の識別子をについて説明します。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ConvertIdResponseMessage](convertidresponsemessage.md) <br/> |状態と[ConvertId の操作](convertid-operation.md)要求の結果が含まれています。  <br/> |
|[SourceIds](sourceids.md) <br/> |変換するソース識別子が含まれます。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>備考

**AlternateId**要素は、2 つの識別子、 [ConvertId 操作](convertid-operation.md)の要求に変換するのには送信元識別子、および[ConvertIdResponse](convertidresponse.md)要素の変換後の識別子について説明します。 
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

||||
|:-----|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目

- [ConvertId 操作](convertid-operation.md)
- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)
- [識別子に変換します。](http://msdn.microsoft.com/library/a5391746-b6ef-4f48-8fc8-8255258651aa%28Office.15%29.aspx)

