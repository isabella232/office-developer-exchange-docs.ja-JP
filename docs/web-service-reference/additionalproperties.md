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
description: AdditionalProperties 要素は、GetItem、UpdateItem、CreateItem FindItem で使用するための追加のプロパティを識別するか、FindFolder 要求します。
ms.openlocfilehash: 64e4f1ee6b24cf8015b7893dc4a904ca8b32d58e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759288"
---
# <a name="additionalproperties"></a>AdditionalProperties

**AdditionalProperties**要素は、 [GetItem](getitem.md)、 [UpdateItem](updateitem.md)、 [CreateItem](createitem.md) [FindItem](finditem.md)で使用するための追加のプロパティを識別するか、 [FindFolder](findfolder.md)要求します。 
  
```xml
<AdditionalProperties>
   <ExtendedFieldURI/>
   <FieldURI/>
   <IndexedFieldURI/>
</AdditionalProperties>
```

 **NonEmptyArrayOfPathsToElementType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[ExtendedFieldURI](extendedfielduri.md) <br/> |取得、設定、または作成する拡張の MAPI プロパティを識別します。  <br/> |
|[FieldURI](fielduri.md) <br/> |URI によって頻繁に参照されるプロパティを識別します。  <br/> |
|[IndexedFieldURI](indexedfielduri.md) <br/> |URI によって頻繁に参照される辞書のプロパティを識別します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[FolderShape](foldershape.md) <br/> | [GetFolder](getfolder.md)、 [FindFolder](findfolder.md)、または[SyncFolderHierarchy](syncfolderhierarchy.md)の応答に含めるフォルダーのプロパティを識別します。<br/><br/>  この要素への XPath 式は、次のように。<br/><br/>  `/FindFolder/FolderShape` <br/>  `/GetFolder/FolderShape` <br/>  `/SyncFolderHierarchy/FolderShape` <br/> |
|[ItemShape](itemshape.md) <br/> | [GetItem](getitem.md)、 [FindItem](finditem.md)、または[SyncFolderItems](syncfolderitems.md)の応答に含めるコンテンツ アイテムのプロパティを識別します。<br/><br/>  この要素への XPath 式は、次のように。<br/><br/>  `/GetItem/ItemShape` <br/>  `/FindItem/ItemShape` <br/>  `/SyncFolderItems/ItemShape` <br/> |
|[AttachmentShape](attachmentshape.md) <br/> |[GetItem](getitem.md)要求への応答で返されるその他の拡張アイテム プロパティを識別します。<br/><br/> この要素への XPath 式は、次のようにします。<br/><br/>  `/GetAttachment/AttachmentShape` <br/> |
   
## <a name="remarks"></a>備考

[GetItem](getitem.md)、 [UpdateItem](updateitem.md)、 [createitem メソッド](createitem.md)、 [FindItem](finditem.md)、 [FindFolder](findfolder.md)要求には、すべての子要素を使用できます。 プロパティは、フォルダーまたはアクセスされているアイテムに適用可能である必要があります。 その他のプロパティにアクセスするのにには、拡張プロパティを使用します。 特定のアイテムのプロパティが存在しない場合は、対応する要素を発しない結果の XML にします。 
  
MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。 
  
この要素はオプションです。
  
## <a name="example"></a>例

要求の次の例では、 **AdditionalProperties**要素を使用して、アイテムの件名を取得する方法を示します。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetItem xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" 
                  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   

