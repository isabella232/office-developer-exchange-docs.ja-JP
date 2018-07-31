---
title: FindFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FindFolder
api_type:
- schema
ms.assetid: b8a59740-d978-454c-9629-a10792385ba0
description: FindFolder 要素は、メールボックス内のフォルダーを検索するための要求を定義します。
ms.openlocfilehash: 69fbaebc5615ac7d19512770658cde83e4d352df
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353533"
---
# <a name="findfolder"></a>FindFolder

**FindFolder**要素は、メールボックス内のフォルダーを検索するための要求を定義します。 
  
```xml
<FindFolder Traversal="Shallow/Deep/SoftDeleted">
   <FolderShape/>
   <IndexedPageFolderView/>
   <Restriction/>
   <ParentFolderIds/>
</FindFolder>
```

```xml
<FindFolder Traversal="Shallow/Deep/SoftDeleted">
   <FolderShape/>
   <FractionalPageFolderView/>
   <Restriction/>
   <ParentFolderIds/>
</FindFolder>
```

**FindFolderType**

## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|トラバーサル  <br/> |検索を実行する方法を定義します。 この属性は、必要があります。  <br/> |
   
#### <a name="traversal-attribute-values"></a>検査の属性値

|**値**|**説明**|
|:-----|:-----|
|浅い  <br/> |識別されたフォルダーのみを検索し、削除されていないアイテムのフォルダー Id のみを取得するために、FindFolder 操作を指示します。 これは簡易走査と呼ばれます。  <br/> |
|深い  <br/> |識別された親フォルダーのすべての子フォルダーで検索して、削除されていないアイテムのフォルダー Id だけを返すには、FindFolder 操作を指示します。 これは、詳細走査と呼ばれます。  <br/> |
|削除済み (回復可能)  <br/> |FindFolder 操作削除済みアイテムの簡易走査の検索を実行するように指示します。  <br/> |
   
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[FolderShape](foldershape.md) <br/> |FindFolder の応答に含めるフォルダーのプロパティを識別します。  <br/> |
|[IndexedPageFolderView](indexedpagefolderview.md) <br/> |どのページの項目の情報について説明します FindFolder 応答が返されます。 この要素はオプションです。  <br/> |
|[FractionalPageFolderView](fractionalpagefolderview.md) <br/> |ページ ビューが起動し、フォルダーの最大数は、FindFolder 要求で返されるについて説明します。 この要素はオプションです。  <br/> |
|[Restriction](restriction.md) <br/> |FindFolder 操作でフォルダーをフィルター処理するために使用されるクエリの制限を定義します。 この要素はオプションです。  <br/> |
|[ParentFolderIds](parentfolderids.md) <br/> |FindFolder 操作が検索するフォルダーを識別します。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="example"></a>例

FindFolder 要求の次の例では、受信トレイ内にあるすべてのフォルダーを検索する要求を作成する方法を示します。
  
```xml
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

