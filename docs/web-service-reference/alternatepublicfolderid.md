---
title: AlternatePublicFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AlternatePublicFolderId
api_type:
- schema
ms.assetid: 0a4dc1cc-959e-4b93-aa3a-3020ca8b8a02
description: AlternatePublicFolderId 要素は、別の識別子の形式に変換するのには、パブリック フォルダーの識別子について説明します。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。
ms.openlocfilehash: 32e6e75eb381e479baf5fdb5ad0a40b32c1b02a9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759319"
---
# <a name="alternatepublicfolderid"></a>AlternatePublicFolderId

**AlternatePublicFolderId**要素は、別の識別子の形式に変換するのには、パブリック フォルダーの識別子について説明します。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。 
  
- [ConvertId](convertid.md)
  
- [SourceIds](sourceids.md)
  
- [AlternatePublicFolderId](alternatepublicfolderid.md)
  
```xml
<AlternatePublicFolderId FolderId="" Format="" />
```

 **AlternatePublicFolderIdType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|フォルダー Id  <br/> |変換するパブリック フォルダーの識別子が含まれています。 この属性は、必要があります。  <br/> |
|Format  <br/> |変換するパブリック フォルダーの識別子を記述する形式を識別します。 この属性は、必要があります。  <br/> |
   
#### <a name="format-attribute"></a>形式の属性

|**値**|**説明**|
|:-----|:-----|
|EwsLegacyId  <br/> |Exchange 2007 の最初のリリース版の Exchange Web サービスによって生成される識別子について説明します。  <br/> |
|EwsId  <br/> |Exchange 2007 SP1 以降の Exchange Web サービスによって生成される識別子について説明します。  <br/> |
|EntryId  <br/> |PR_ENTRYID プロパティと同様に、MAPI 識別子をについて説明します。  <br/> |
|HexEntryId  <br/> |PR_ENTRYID プロパティの 16 進数でエンコードされた表現を説明します。 これは、可用性の予定表のイベント識別子の形式です。  <br/> |
|StoreId  <br/> |Exchange ストア識別子をについて説明します。  <br/> |
|OwaId  <br/> |Outlook Web Access 識別子をについて説明します。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[SourceIds](sourceids.md) <br/> |変換するソース識別子が含まれます。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。  <br/> |
   
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |True  <br/> |
   
## <a name="see-also"></a>関連項目

- [ConvertId 操作](convertid-operation.md)
- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)
- [識別子に変換します。](http://msdn.microsoft.com/library/a5391746-b6ef-4f48-8fc8-8255258651aa%28Office.15%29.aspx)

