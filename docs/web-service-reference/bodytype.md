---
title: BodyType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- BodyType
api_type:
- schema
ms.assetid: d42ec77b-fb9f-404a-9bf2-1801e8744676
description: BodyType 要素は、本文テキストが応答で書式設定される方法を識別します。
ms.openlocfilehash: e8952ac2774589e031280ce982ea8671b736a87d
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59526842"
---
# <a name="bodytype"></a>BodyType

**BodyType 要素** は、本文テキストが応答で書式設定される方法を識別します。 
  
```xml
<BodyType>Best or HTML or Text</BodyType>
```

**BodyTypeResponseType**

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ItemShape](itemshape.md) <br/> | GetItem、FindItem、または SyncFolderItems 応答に含めるアイテムのプロパティとコンテンツを識別します。  <br/><br/>この要素の XPath 式を次に示します。<br/><br/>  `/GetItem/ItemShape`<br/><br/>`/FindItem/ItemShape`<br/><br/>`/SyncFolderItems/ItemShape` <br/> |
|[AttachmentShape](attachmentshape.md) <br/> |[GetAttachment](getattachment.md)要求への応答で返す追加の拡張アイテム プロパティを識別します。  <br/><br/>次に、この要素の XPath 式を示します。<br/><br/>  `/GetAttachment/AttachmentShape` <br/> |
   
## <a name="text-value"></a>テキスト値

次の表に **、BodyType** 要素に使用できる値を示します。 
  
|**値**|**説明**|
|:-----|:-----|
|高  <br/> |応答は、本文テキストの利用可能な最もリッチなコンテンツを返します。 これは、コンテンツがテキストか HTML か不明な場合に便利です。<br/><br/> 格納された本文がプレーン テキストの場合、返される本文はテキストです。 それ以外の場合、格納されている本文が HTML 形式または RTF 形式の場合、応答は HTML を返します。<br/><br/> これが既定値です。  <br/> |
|HTML  <br/> |応答は、アイテムの本文を HTML として返します。  <br/> |
|テキスト  <br/> |応答は、アイテム本文をプレーン テキストとして返します。  <br/> |
   
## <a name="remarks"></a>注釈

Body 要素の **BodyType** 属性を調べ、応答で返される本文の種類を [識別](body.md) できます。 **BodyType 属性** は、本文を HTML またはテキストとして識別します。 
  
この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている MicrosoftExchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="example"></a>例

次の要求の例は、BodyType 要素が使用 **される場所を** 示しています。 
  
```xml
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetAttachment xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <AttachmentShape>
        <t:BodyType>Best</t:BodyType>
      </AttachmentShape>
      <AttachmentIds>
        <t:AttachmentId Id="ASkAS="/>
      </AttachmentIds>
    </GetAttachment>
  </soap:Body>
</soap:Envelope>
```

Id 属性は、読みやすさを維持するために短縮されました。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   

