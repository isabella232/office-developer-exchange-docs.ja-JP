---
title: AlternatePublicFolderItemId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AlternatePublicFolderItemId
api_type:
- schema
ms.assetid: a67df9b9-8fdb-42de-b9c5-8377b71fa3d9
description: AlternatePublicFolderItemId 要素は、別の識別子形式に変換するためのパブリックフォルダーアイテム識別子を表します。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。
ms.openlocfilehash: 11a9fafec78a9bd14e4d98982fd38954d45e4d1a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44464771"
---
# <a name="alternatepublicfolderitemid"></a>AlternatePublicFolderItemId

**Alternatepublicfolderitemid**要素は、別の識別子形式に変換するためのパブリックフォルダーアイテム識別子を表します。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。 
  
- [ConvertId](convertid.md)
  
- [SourceIds](sourceids.md)
  
- [AlternatePublicFolderItemId](alternatepublicfolderitemid.md)
  
```xml
<AlternatePublicFolderItemId FolderId="" Format="" ItemId=""/>
```

 **AlternatePublicFolderItemIdType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|FolderId  <br/> |パブリックフォルダーアイテムを含むパブリックフォルダーを識別します。 この属性は必須です。  <br/> |
|Format  <br/> |変換するパブリックフォルダーアイテム識別子を説明する形式を識別します。 この属性は必須です。  <br/> |
|ItemId  <br/> |識別子変換するパブリックフォルダーアイテム。 この属性は必須です。  <br/> |
   
#### <a name="format-attribute-values"></a>書式属性値

|**値**|**説明**|
|:-----|:-----|
|EwsLegacyId  <br/> |Exchange 2007 の最初のリリースバージョンで Exchange Web サービスによって生成された識別子について説明します。  <br/> |
|EwsId  <br/> |Exchange 2007 SP1 以降の Exchange Web サービスによって生成される識別子について説明します。  <br/> |
|EntryId  <br/> |PR_ENTRYID プロパティのように、MAPI 識別子について説明します。  <br/> |
|HexEntryId  <br/> |PR_ENTRYID プロパティの16進数でエンコードされた表現を記述します。 これは、可用性カレンダーイベント識別子の形式です。  <br/> |
|StoreId  <br/> |Exchange ストア識別子について説明します。  <br/> |
|OwaId  <br/> |Outlook Web Access 識別子を表します。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[SourceIds](sourceids.md) <br/> |変換するソース識別子を含みます。 この要素は、Exchange 2007 SP1 で導入されました。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しい  <br/> |
   
## <a name="see-also"></a>関連項目

- [ConvertId 操作](convertid-operation.md)
- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)
- [識別子の変換](https://msdn.microsoft.com/library/a5391746-b6ef-4f48-8fc8-8255258651aa%28Office.15%29.aspx)

