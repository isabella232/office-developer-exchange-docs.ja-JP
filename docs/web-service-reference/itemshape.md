---
title: ItemShape
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ItemShape
api_type:
- schema
ms.assetid: c5604161-bbc0-40bc-ad75-ff7e837d745f
description: ItemShape 要素は、GetItem 操作、FindItem 操作、または SyncFolderItems 操作の応答で返される一連のプロパティを識別します。
ms.openlocfilehash: ffb666ee331b55a4f04cad076c705e4bec980e03
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458125"
---
# <a name="itemshape"></a>ItemShape

**Itemshape**要素は、 [GetItem 操作](getitem-operation.md)、 [FindItem 操作](finditem-operation.md)、または[syncfolderitems 操作](syncfolderitems-operation.md)の応答で返される一連のプロパティを識別します。 
  
```XML
<ItemShape>
   <BaseShape/>
   <IncludeMimeContent/>
   <BodyType/>
   <FilterHtmlContent/>
   <ConvertHtmlCodePageToUTF8/>
   <AdditionalProperties/>
</ItemShape>
```

 **ItemResponseShapeType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[BaseShape](baseshape.md) <br/> |アイテムまたはフォルダーの応答で返されるプロパティの基本的な構成を識別します。  <br/> |
|[IncludeMimeContent](includemimecontent.md) <br/> |アイテムのマルチパーパスインターネットメール内線 (MIME) コンテンツを応答で返すかどうかを指定します。  <br/> |
|[BodyType](bodytype.md) <br/> |応答で本文テキストを書式設定する方法を指定します。  <br/> |
|[ConvertHtmlCodePageToUTF8](converthtmlcodepagetoutf8.md) <br/> |アイテムの HTML 本文を UTF8 に変換するかどうかを示します。  <br/> |
|[FilterHtmlContent](filterhtmlcontent.md) <br/> |HTML コンテンツフィルターを有効にするかどうかを指定します。  <br/> |
|[AdditionalProperties](additionalproperties.md) <br/> |応答で返される追加のプロパティを識別します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[GetItem](getitem.md) <br/> |Exchange ストア内のメールボックスからアイテムを取得するための要求を定義します。  <br/> この要素の XPath 式を次に示します。  <br/>  `/GetItem` <br/> |
|[FindItem](finditem.md) <br/> |フォルダーに含まれるすべてのアイテムを検索するための要求を定義します。  <br/> この要素の XPath 式を次に示します。  <br/>  `/FindItem` <br/> |
|[SyncFolderItems](syncfolderitems.md) <br/> |Exchange ストアフォルダー内のアイテムを同期する要求を定義します。  <br/> この要素の XPath 式を次に示します。  <br/>  `/SyncFolderItems` <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



[GetItem 操作](getitem-operation.md)
  
[FindItem 操作](finditem-operation.md)
  
[SyncFolderItems 操作](syncfolderitems-operation.md)


- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

