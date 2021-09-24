---
title: AdditionalProperties
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- AdditionalProperties
api_type:
- schema
ms.assetid: 7a269aed-dcfd-4c3e-9e14-094e53828101
description: AdditionalProperties 要素は、GetItem、UpdateItem、CreateItem、FindItem、または FindFolder 要求で使用する追加のプロパティを識別します。
ms.openlocfilehash: 9a6fb98e9a88b1e40bd83559b1836d4122f0f125
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59522202"
---
# <a name="additionalproperties"></a>AdditionalProperties

**AdditionalProperties 要素は**[、GetItem、UpdateItem、CreateItem、FindItem、](getitem.md)または [](finditem.md)[FindFolder](findfolder.md)要求で使用する追加のプロパティを識別します。 [](updateitem.md) [](createitem.md) 
  
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
|[FieldURI](fielduri.md) <br/> |URI によって頻繁に参照されるプロパティを識別します。  <br/> |
|[IndexedFieldURI](indexedfielduri.md) <br/> |URI によって頻繁に参照される辞書プロパティを識別します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[FolderShape](foldershape.md) <br/> | [GetFolder、FindFolder、または](getfolder.md) [SyncFolderHierarchy](syncfolderhierarchy.md)応答に含めるフォルダー プロパティを識別します。 [](findfolder.md)<br/><br/>  この要素の XPath 式を次に示します。<br/><br/>  `/FindFolder/FolderShape` <br/>  `/GetFolder/FolderShape` <br/>  `/SyncFolderHierarchy/FolderShape` <br/> |
|[ItemShape](itemshape.md) <br/> | [GetItem、FindItem、または](getitem.md) [SyncFolderItems](syncfolderitems.md) [](finditem.md)応答に含めるアイテムのプロパティとコンテンツを識別します。<br/><br/>  この要素の XPath 式を次に示します。<br/><br/>  `/GetItem/ItemShape` <br/>  `/FindItem/ItemShape` <br/>  `/SyncFolderItems/ItemShape` <br/> |
|[AttachmentShape](attachmentshape.md) <br/> |GetItem 要求への応答で返す追加の拡張アイテム プロパティ [を識別](getitem.md) します。<br/><br/> 次に、この要素の XPath 式を示します。<br/><br/>  `/GetAttachment/AttachmentShape` <br/> |
   
## <a name="remarks"></a>注釈

[GetItem、UpdateItem、CreateItem、FindItem、](updateitem.md)[または](finditem.md) [FindFolder](findfolder.md)要求ですべての子要素を使用できるということはありません。 [](getitem.md) [](createitem.md) プロパティは、アクセスされるフォルダーまたはアイテムに適用できる必要があります。 他のプロパティにアクセスするには、拡張プロパティを使用します。 特定のアイテムに対してプロパティが存在しない場合、対応する要素は結果の XML に出力されません。 
  
この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている MicrosoftExchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。 
  
この要素は省略できます。
  
## <a name="example"></a>例

次の要求例は、AdditionalProperties 要素を使用してアイテムの件名を **取得する方法を示** しています。 
  
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
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   

