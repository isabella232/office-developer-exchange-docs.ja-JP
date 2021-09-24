---
title: AlternatePublicFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- AlternatePublicFolderId
api_type:
- schema
ms.assetid: 0a4dc1cc-959e-4b93-aa3a-3020ca8b8a02
description: AlternatePublicFolderId 要素は、別の識別子形式に変換するパブリック フォルダー識別子について説明します。 この要素は、2007 Microsoft Exchange Server パック 1 (SP1) で導入されました。
ms.openlocfilehash: 7c4471c0c1e3e1eee3b47eba42f924340891c777
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59525359"
---
# <a name="alternatepublicfolderid"></a>AlternatePublicFolderId

**AlternatePublicFolderId** 要素は、別の識別子形式に変換するパブリック フォルダー識別子について説明します。 この要素は、2007 Microsoft Exchange Server パック 1 (SP1) で導入されました。 
  
- [ConvertId](convertid.md)
  
- [SourceIds](sourceids.md)
  
- [AlternatePublicFolderId](alternatepublicfolderid.md)
  
```xml
<AlternatePublicFolderId FolderId="" Format="" />
```

 **AlternatePublicFolderIdType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|FolderId  <br/> |変換するパブリック フォルダー識別子が含まれる。 この属性は必須です。  <br/> |
|フォーマット  <br/> |変換するパブリック フォルダー識別子を記述する形式を識別します。 この属性は必須です。  <br/> |
   
#### <a name="format-attribute"></a>Format 属性

|**値**|**説明**|
|:-----|:-----|
|EwsLegacyId  <br/> |2007 年の初期リリース バージョンExchange Web サービスによって生成される識別子Exchangeします。  <br/> |
|EwsId  <br/> |2007 SP1 から始まる Web サービスExchange生成されるExchange説明します。  <br/> |
|EntryId  <br/> |MAPI 識別子について説明します。このプロパティPR_ENTRYIDします。  <br/> |
|HexEntryId  <br/> |プロパティの 16 進数でエンコードされた表現PR_ENTRYIDします。 これは、利用可能な予定表のイベント識別子の形式です。  <br/> |
|StoreId  <br/> |ストアExchangeについて説明します。  <br/> |
|OwaId  <br/> |Web アクセス識別子Outlook説明します。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[SourceIds](sourceids.md) <br/> |変換するソース識別子が含まれる。 この要素は、2007 Microsoft Exchange Server パック 1 (SP1) で導入されました。  <br/> |
   
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |正解  <br/> |
   
## <a name="see-also"></a>関連項目

- [ConvertId 操作](convertid-operation.md)
- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)
- [識別子の変換](https://msdn.microsoft.com/library/a5391746-b6ef-4f48-8fc8-8255258651aa%28Office.15%29.aspx)

