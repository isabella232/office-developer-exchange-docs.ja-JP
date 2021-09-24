---
title: BaseShape
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- BaseShape
api_type:
- schema
ms.assetid: 42c04f3b-abaa-4197-a3d6-d21677ffb1c0
description: BaseShape 要素は、アイテムまたはフォルダーの応答で返すプロパティのセットを識別します。
ms.openlocfilehash: b4e7f5c6d6520e7338f274b6275e371366b1bed5
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59514859"
---
# <a name="baseshape"></a>BaseShape

**BaseShape 要素は**、アイテムまたはフォルダーの応答で返すプロパティのセットを識別します。 
  
```xml
<BaseShape>IdOnly or Default or AllProperties</BaseShape>
```

 **DefaultShapeNamesType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[FolderShape](foldershape.md) <br/> | GetFolder、FindFolder、または SyncFolderHierarchy 応答に含めるフォルダー プロパティを識別します。<br/><br/>この要素の XPath 式を次に示します。<br/><br/>`/GetFolder/FolderShape` <br/>  `/FindFolder/FolderShape` <br/>  `/SyncFolderHierarchy/FolderShape` <br/> |
|[ItemShape](itemshape.md) <br/> | GetItem、FindItem、または SyncFolderItems 応答に含めるアイテムのプロパティとコンテンツを識別します。<br/><br/>この要素の XPath 式を次に示します。<br/><br/>`/GetItem/ItemShape` <br/>  `/FindItem/ItemShape` <br/>  `/SyncFolderItems/ItemShape` <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は必須です。 次の表に、使用可能なテキスト値を示します。
  
**BaseShape 要素のテキスト値**

|**値**|**説明**|
|:-----|:-----|
|IdOnly  <br/> |アイテムまたはフォルダー ID のみを返します。  <br/> |
|既定値  <br/> |アイテムまたはフォルダーの既定として定義されているプロパティのセットを返します。  <br/> |
|AllProperties  <br/> |ビジネス ロジックレイヤーでフォルダーを作成するために使用Exchangeプロパティを返します。  <br/> |
   
次の表に、FindFolder 要求に対して返される既定のプロパティを示します。 指定したフォルダーのすべてのサブフォルダーは、名前順に返されます。
  
**既定のプロパティ**

|**Folder**|**既定のプロパティ**|
|:-----|:-----|
|受信トレイ  <br/> |FolderId、表示名、未読数、合計カウント、サブフォルダー数  <br/> |
|連絡先  <br/> |FolderId、表示名、合計カウント、サブフォルダー数  <br/> |
|予定表  <br/> |FolderId、表示名、サブフォルダー数  <br/> |
|下書き  <br/> |FolderId、表示名、未読数、合計カウント、サブフォルダー数  <br/> |
|削除済みアイテム  <br/> |FolderId、表示名、未読数、合計カウント、サブフォルダー数  <br/> |
|その他のフォルダー  <br/> |FolderId、表示名、未読数、合計カウント、サブフォルダー数  <br/> |
|送信トレイ  <br/> |FolderId、表示名、未読数、合計カウント、サブフォルダー数  <br/> |
|タスク  <br/> |FolderId、表示名、過去の期限数、合計カウント、サブフォルダー数  <br/> |
|メモ  <br/> |FolderId、表示名、合計カウント、サブフォルダー数  <br/> |
   
## <a name="remarks"></a>注釈

[BaseShape](baseshape.md)要素で識別されるプロパティに加えてプロパティを返す場合は[、AdditionalProperties 要素を使用](additionalproperties.md)します。 
  
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
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目

- [FolderShape](foldershape.md)
- [ItemShape](itemshape.md)

