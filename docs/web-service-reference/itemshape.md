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
description: ItemShape 要素は、GetItem 操作、FindItem 操作、または SyncFolderItems 操作の応答で返されるプロパティのセットを識別します。
ms.openlocfilehash: 95174a85a8fa05cb2612e1289d46c8db32b6e052
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832191"
---
# <a name="itemshape"></a>ItemShape

**ItemShape**要素は、 [GetItem 操作](getitem-operation.md)、 [FindItem 操作](finditem-operation.md)、または[SyncFolderItems の操作](syncfolderitems-operation.md)の応答で返されるプロパティのセットを識別します。 
  
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
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[BaseShape](baseshape.md) <br/> |アイテムまたはフォルダーの応答で返されるプロパティの基本構成を識別します。  <br/> |
|[IncludeMimeContent](includemimecontent.md) <br/> |応答で、多目的インターネット メール拡張 (MIME) のコンテンツ項目を返すかどうかを指定します。  <br/> |
|[BodyType](bodytype.md) <br/> |応答の本文のテキストを書式設定する方法を識別します。  <br/> |
|[ConvertHtmlCodePageToUTF8](converthtmlcodepagetoutf8.md) <br/> |項目の HTML 本文が UTF8 に変換されるかどうかを示します。  <br/> |
|[FilterHtmlContent](filterhtmlcontent.md) <br/> |HTML コンテンツのフィルタ リングが有効になっているかどうかを指定します。  <br/> |
|[AdditionalProperties](additionalproperties.md) <br/> |応答で返される追加プロパティを識別します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[GetItem](getitem.md) <br/> |Exchange ストア内のメールボックスからアイテムを取得する要求を定義します。  <br/> この要素への XPath 式は、次のようにします。  <br/>  `/GetItem` <br/> |
|[FindItem](finditem.md) <br/> |フォルダーに含まれるすべての項目を検索するための要求を定義します。  <br/> この要素への XPath 式は、次のようにします。  <br/>  `/FindItem` <br/> |
|[SyncFolderItems](syncfolderitems.md) <br/> |Exchange ストア フォルダー内のアイテムを同期するための要求を定義します。  <br/> この要素への XPath 式は、次のようにします。  <br/>  `/SyncFolderItems` <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>備考

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目




  [GetItem 操作](getitem-operation.md)
  

  [FindItem 操作](finditem-operation.md)
  
[SyncFolderItems の操作](syncfolderitems-operation.md)


- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

