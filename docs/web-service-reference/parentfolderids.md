---
title: ParentFolderIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ParentFolderIds
api_type:
- schema
ms.assetid: e7998023-e5e0-465c-91fa-2aa6d1559f64
description: ParentFolderIds 要素は、検索 FindItem と FindFolder 操作用のフォルダーを識別します。
ms.openlocfilehash: 4dd23b45dcc397e29e67fc08b29dd773e50f0db1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832688"
---
# <a name="parentfolderids"></a>ParentFolderIds

**ParentFolderIds**要素は、検索 FindItem と FindFolder 操作用のフォルダーを識別します。 
  
```xml
<ParentFolderIds>
   <DistinguishedFolderId/>
<ParentFolderIds>
```

**NonEmptyArrayOfBaseFolderIdsType**

## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[フォルダー Id](folderid.md) <br/> |フォルダーの識別子と変更キーが含まれています。 **ParentFolderIds**要素には、この要素または[DistinguishedFolderId](distinguishedfolderid.md)要素のいずれかを使用する必要があります。  <br/> |
|[DistinguishedFolderId](distinguishedfolderid.md) <br/> |名前で参照できる Microsoft Exchange Server 2007 のフォルダーを識別します。 **ParentFolderIds**要素には、[フォルダー Id](folderid.md)要素またはこの要素のいずれかを使用する必要があります。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[FindFolder](findfolder.md) <br/> |メールボックス内のフォルダーを識別するための要求を定義します。  <br/> |
|[FindItem](finditem.md) <br/> |メールボックス内のアイテムを検索するための要求を定義します。  <br/> |
|[ResolveNames](resolvenames.md) <br/> |あいまいな名前を解決する要求を定義します。  <br/> |
   
## <a name="remarks"></a>備考

**ParentFolderIds**要素には、[フォルダー Id](folderid.md)または[DistinguishedFolderId](distinguishedfolderid.md)要素のいずれかを使用する必要があります。 検索対象のフォルダーの無制限の数を定義できます。 
  
## <a name="example"></a>例

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindFolder Traversal="Shallow" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <FolderShape>
        <t:BaseShape>Default</t:BaseShape>
      </FolderShape>
      <ParentFolderIds>
        <t:DistinguishedFolderId Id="inbox"/>
      </ParentFolderIds>
    </FindFolder>
  </soap:Body>
</soap:Envelope>
```

## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目

- 
  [FindFolder 操作](findfolder-operation.md)  
- 
  [FindItem 操作](finditem-operation.md) 
- [ResolveNames 操作](resolvenames-operation.md)

