---
title: ParentFolderIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ParentFolderIds
api_type:
- schema
ms.assetid: e7998023-e5e0-465c-91fa-2aa6d1559f64
description: ParentFolderIds 要素は、検索する FindItem 操作と FindFolder 操作のフォルダーを識別します。
ms.openlocfilehash: e9e0f14651b205ad64be04dbe1d0707a109f3edc
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59512906"
---
# <a name="parentfolderids"></a>ParentFolderIds

**ParentFolderIds 要素は**、検索する FindItem 操作と FindFolder 操作のフォルダーを識別します。 
  
```xml
<ParentFolderIds>
   <DistinguishedFolderId/>
<ParentFolderIds>
```

```xml
<ParentFolderIds>
   <FolderId/> 
<ParentFolderIds>
```

**NonEmptyArrayOfBaseFolderIdsType**

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[FolderId](folderid.md) <br/> |フォルダーの識別子と変更キーを格納します。 **ParentFolderIds 要素** は、この要素または [DistinguishedFolderId 要素のいずれかを使用する必要](distinguishedfolderid.md)があります。  <br/> |
|[DistinguishedFolderId](distinguishedfolderid.md) <br/> |名前でMicrosoft Exchange Serverできる 2007 フォルダーを識別します。 **ParentFolderIds 要素** は、この要素または FolderId 要素のいずれかを使用 [する必要](folderid.md)があります。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[FindFolder](findfolder.md) <br/> |メールボックス内のフォルダーを識別するための要求を定義します。  <br/> |
|[FindItem](finditem.md) <br/> |メールボックス内のアイテムを検索する要求を定義します。  <br/> |
|[ResolveNames](resolvenames.md) <br/> |あいまいな名前を解決するための要求を定義します。  <br/> |
   
## <a name="remarks"></a>注釈

**ParentFolderIds 要素** は [、FolderId](folderid.md)または [DistinguishedFolderId 要素のいずれかを使用する必要](distinguishedfolderid.md)があります。 検索には、無制限の数のフォルダーを定義できます。 
  
## <a name="example"></a>例

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindFolder Traversal="Shallow" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目

- [FindFolder 操作](findfolder-operation.md)  
- [FindItem 操作](finditem-operation.md) 
- [ResolveNames 操作](resolvenames-operation.md)

