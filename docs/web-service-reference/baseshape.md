---
title: BaseShape
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- BaseShape
api_type:
- schema
ms.assetid: 42c04f3b-abaa-4197-a3d6-d21677ffb1c0
description: BaseShape の要素は、アイテムまたはフォルダーの応答で返されるプロパティのセットを識別します。
ms.openlocfilehash: 69b27d23fd75d4c1a274f31dfa419b759dbb2bbe
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759497"
---
# <a name="baseshape"></a>BaseShape

**BaseShape**の要素は、アイテムまたはフォルダーの応答で返されるプロパティのセットを識別します。 
  
```xml
<BaseShape>IdOnly or Default or AllProperties</BaseShape>
```

 **DefaultShapeNamesType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[FolderShape](foldershape.md) <br/> | GetFolder、FindFolder、または SyncFolderHierarchy の応答に含めるフォルダーのプロパティを識別します。<br/><br/>この要素への XPath 式は、次のように。<br/><br/>`/GetFolder/FolderShape` <br/>  `/FindFolder/FolderShape` <br/>  `/SyncFolderHierarchy/FolderShape` <br/> |
|[ItemShape](itemshape.md) <br/> | GetItem、FindItem、または SyncFolderItems の応答に含めるコンテンツ アイテムのプロパティを識別します。<br/><br/>この要素への XPath 式は、次のように。<br/><br/>`/GetItem/ItemShape` <br/>  `/FindItem/ItemShape` <br/>  `/SyncFolderItems/ItemShape` <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は必須です。 次の表は、可能なテキスト値を示します。
  
**BaseShape 要素のテキスト値**

|**値**|**説明**|
|:-----|:-----|
|IdOnly  <br/> |アイテムまたはフォルダーの ID を返します。  <br/> |
|Default  <br/> |アイテムまたはフォルダーの既定値として定義されているプロパティのセットを返します。  <br/> |
|AllProperties  <br/> |フォルダーを作成するのには、Exchange ビジネス ロジック層で使用されるすべてのプロパティを返します。  <br/> |
   
FindFolder 要求に対して返される既定のプロパティを次の表に一覧します。 名前の順序で指定されたフォルダーのすべてのサブフォルダーが返されます。
  
**既定のプロパティ**

|**Folder**|**既定のプロパティ**|
|:-----|:-----|
|受信トレイ  <br/> |フォルダー Id、表示名、未読数、合計数、サブフォルダーの数  <br/> |
|連絡先  <br/> |フォルダー Id、表示名、合計数、サブフォルダーの数  <br/> |
|カレンダー  <br/> |フォルダー Id、表示名、サブフォルダーの数  <br/> |
|������  <br/> |フォルダー Id、表示名、未読数、合計数、サブフォルダーの数  <br/> |
|削除済みアイテム  <br/> |フォルダー Id、表示名、未読数、合計数、サブフォルダーの数  <br/> |
|その他のフォルダー  <br/> |フォルダー Id、表示名、未読数、合計数、サブフォルダーの数  <br/> |
|送信トレイ  <br/> |フォルダー Id、表示名、未読数、合計数、サブフォルダーの数  <br/> |
|タスク  <br/> |フォルダー Id、表示名、期限経過のカウント、合計、サブフォルダーの数  <br/> |
|���l  <br/> |フォルダー Id、表示名、合計数、サブフォルダーの数  <br/> |
   
## <a name="remarks"></a>備考

[BaseShape](baseshape.md)の要素で指定されたもの以外のプロパティを取得するには、 [AdditionalProperties](additionalproperties.md)要素を使用します。 
  
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
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目

- [FolderShape](foldershape.md)
- [ItemShape](itemshape.md)

