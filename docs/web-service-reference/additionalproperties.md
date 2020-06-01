---
title: AdditionalProperties
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AdditionalProperties
api_type:
- schema
ms.assetid: 7a269aed-dcfd-4c3e-9e14-094e53828101
description: AdditionalProperties 要素は、GetItem、UpdateItem、CreateItem、FindItem、または FindFolder 要求で使用する追加のプロパティを示します。
ms.openlocfilehash: 90a307ba4d5ece10e15d2cec56cf5042c3d38685
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455815"
---
# <a name="additionalproperties"></a>AdditionalProperties

**Additionalproperties**要素は、 [GetItem](getitem.md)、 [updateitem](updateitem.md)、 [CreateItem](createitem.md)、 [FindItem](finditem.md)、または[findfolder](findfolder.md)要求で使用する追加のプロパティを示します。 
  
```xml
<AdditionalProperties>
   <ExtendedFieldURI/>
   <FieldURI/>
   <IndexedFieldURI/>
</AdditionalProperties>
```

 **NonEmptyArrayOfPathsToElementType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[ExtendedFieldURI](extendedfielduri.md) <br/> |取得、設定、または作成する拡張 MAPI プロパティを識別します。  <br/> |
|[FieldURI](fielduri.md) <br/> |URI で頻繁に参照されるプロパティを識別します。  <br/> |
|[IndexedFieldURI](indexedfielduri.md) <br/> |URI で頻繁に参照される dictionary プロパティを識別します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[FolderShape](foldershape.md) <br/> | [Getfolder](getfolder.md)、 [findfolder](findfolder.md)、または[syncfolderhierarchy](syncfolderhierarchy.md)の応答に含めるフォルダーのプロパティを識別します。<br/><br/>  この要素の XPath 式は次のとおりです。<br/><br/>  `/FindFolder/FolderShape` <br/>  `/GetFolder/FolderShape` <br/>  `/SyncFolderHierarchy/FolderShape` <br/> |
|[ItemShape](itemshape.md) <br/> | [GetItem](getitem.md)、 [FindItem](finditem.md)、または[syncfolderitems](syncfolderitems.md)応答に含めるアイテムのプロパティとコンテンツを指定します。<br/><br/>  この要素の XPath 式は次のとおりです。<br/><br/>  `/GetItem/ItemShape` <br/>  `/FindItem/ItemShape` <br/>  `/SyncFolderItems/ItemShape` <br/> |
|[AttachmentShape](attachmentshape.md) <br/> |[GetItem](getitem.md)要求に対する応答で返される追加の拡張アイテムプロパティを識別します。<br/><br/> この要素の XPath 式を次に示します。<br/><br/>  `/GetAttachment/AttachmentShape` <br/> |
   
## <a name="remarks"></a>注釈

[GetItem](getitem.md)、 [updateitem](updateitem.md)、 [CreateItem](createitem.md)、 [FindItem](finditem.md)、または[findfolder](findfolder.md)要求では、すべての子要素を使用できるわけではありません。 このプロパティは、アクセスされるフォルダーまたはアイテムに適用される必要があります。 他のプロパティにアクセスするには、拡張プロパティを使用します。 指定したアイテムのプロパティが存在しない場合、対応する要素は結果の XML に出力されません。 
  
この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。 
  
この要素は省略できます。
  
## <a name="example"></a>例

次の要求例は、 **Additionalproperties**要素を使用してアイテムの件名を取得する方法を示しています。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetItem xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" 
                  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Subject"/>
        </t:AdditionalProperties>
      </ItemShape>
      <ItemIds>
        <t:ItemId Id="ASkAS="/>
      </ItemIds>
    </GetItem>
  </soap:Body>
</soap:Envelope>
```

## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   

