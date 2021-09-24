---
title: ItemShape
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ItemShape
api_type:
- schema
ms.assetid: c5604161-bbc0-40bc-ad75-ff7e837d745f
description: ItemShape 要素は、GetItem 操作、FindItem 操作、または SyncFolderItems 操作応答で返すプロパティのセットを識別します。
ms.openlocfilehash: d6cc1efc85a8a22e12f2a3616fe949b72b3bba33
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59519395"
---
# <a name="itemshape"></a>ItemShape

**ItemShape 要素は**[、GetItem 操作、FindItem](getitem-operation.md)操作、または [](finditem-operation.md)[SyncFolderItems](syncfolderitems-operation.md)操作応答で返すプロパティのセットを識別します。 
  
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
|[BaseShape](baseshape.md) <br/> |アイテムまたはフォルダーの応答で返すプロパティの基本的な構成を識別します。  <br/> |
|[IncludeMimeContent](includemimecontent.md) <br/> |アイテムの多目的インターネット メール拡張機能 (MIME) コンテンツを応答で返すかどうかを指定します。  <br/> |
|[BodyType](bodytype.md) <br/> |本文テキストが応答で書式設定される方法を識別します。  <br/> |
|[ConvertHtmlCodePageToUTF8](converthtmlcodepagetoutf8.md) <br/> |アイテム HTML 本文が UTF8 に変換されるかどうかを示します。  <br/> |
|[FilterHtmlContent](filterhtmlcontent.md) <br/> |HTML コンテンツ フィルターを有効にするかどうかを指定します。  <br/> |
|[AdditionalProperties](additionalproperties.md) <br/> |応答で返す追加のプロパティを識別します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[GetItem](getitem.md) <br/> |メールボックス ストア内のメールボックスからアイテムを取得する要求Exchangeします。  <br/> 次に、この要素の XPath 式を示します。  <br/>  `/GetItem` <br/> |
|[FindItem](finditem.md) <br/> |フォルダーに含まれるすべてのアイテムを検索する要求を定義します。  <br/> 次に、この要素の XPath 式を示します。  <br/>  `/FindItem` <br/> |
|[SyncFolderItems](syncfolderitems.md) <br/> |ストア フォルダー内のアイテムを同期する要求Exchange定義します。  <br/> 次に、この要素の XPath 式を示します。  <br/>  `/SyncFolderItems` <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



[GetItem 操作](getitem-operation.md)
  
[FindItem 操作](finditem-operation.md)
  
[SyncFolderItems 操作](syncfolderitems-operation.md)


- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

