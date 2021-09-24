---
title: FindFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- FindFolder
api_type:
- schema
ms.assetid: b8a59740-d978-454c-9629-a10792385ba0
description: FindFolder 要素は、メールボックス内のフォルダーを検索する要求を定義します。
ms.openlocfilehash: 431efde28e417efec04f6fa1625a81b3766cb705
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59518443"
---
# <a name="findfolder"></a>FindFolder

**FindFolder 要素は**、メールボックス内のフォルダーを検索する要求を定義します。 
  
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

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|Traversal  <br/> |検索の実行方法を定義します。 この属性は必須です。  <br/> |
   
#### <a name="traversal-attribute-values"></a>Traversal 属性値

|**値**|**説明**|
|:-----|:-----|
|浅い  <br/> |FindFolder 操作で、識別されたフォルダーのみを検索し、削除されていないアイテムのフォルダーの ID のみを返すよう指示します。 これを浅いトラバーサルと呼ぶ。  <br/> |
|深い  <br/> |FindFolder 操作で、識別された親フォルダーのすべての子フォルダーを検索し、削除されていないアイテムのフォルダーの ID のみを返すよう指示します。 これをディープ トラバーサルと呼ぶ。  <br/> |
|削除済み (回復可能)  <br/> |FindFolder 操作に、削除済みアイテムの浅いトラバーサル検索を実行するように指示します。  <br/> |
   
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[FolderShape](foldershape.md) <br/> |FindFolder 応答に含めるフォルダー プロパティを識別します。  <br/> |
|[IndexedPageFolderView](indexedpagefolderview.md) <br/> |FindFolder 応答でページアイテム情報がどのように返されるのかについて説明します。 この要素は省略できます。  <br/> |
|[FractionalPageFolderView](fractionalpagefolderview.md) <br/> |ページ ビューの開始場所と FindFolder 要求で返されるフォルダーの最大数について説明します。 この要素は省略できます。  <br/> |
|[Restriction](restriction.md) <br/> |FindFolder 操作でフォルダーをフィルター処理するために使用する制限またはクエリを定義します。 この要素は省略できます。  <br/> |
|[ParentFolderIds](parentfolderids.md) <br/> |検索する FindFolder 操作のフォルダーを識別します。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="example"></a>例

FindFolder 要求の次の例は、受信トレイ内のすべてのフォルダーを検索する要求を形成する方法を示しています。
  
```xml
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

