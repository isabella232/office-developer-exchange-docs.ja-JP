---
title: BodyType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- BodyType
api_type:
- schema
ms.assetid: d42ec77b-fb9f-404a-9bf2-1801e8744676
description: BodyType 要素は、本文テキストがどのように応答で書式設定されるかを識別します。
ms.openlocfilehash: 448d20ac54b09a2f4f6a273a1099519371ac7f5b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465948"
---
# <a name="bodytype"></a>BodyType

**Bodytype**要素は、本文テキストがどのように応答で書式設定されるかを識別します。 
  
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
|[ItemShape](itemshape.md) <br/> | GetItem、FindItem、または SyncFolderItems 応答に含めるアイテムのプロパティとコンテンツを指定します。  <br/><br/>この要素の XPath 式は次のとおりです。<br/><br/>  `/GetItem/ItemShape`<br/><br/>`/FindItem/ItemShape`<br/><br/>`/SyncFolderItems/ItemShape` <br/> |
|[AttachmentShape](attachmentshape.md) <br/> |[Getattachment](getattachment.md)要求に対する応答で返される追加の拡張アイテムプロパティを識別します。  <br/><br/>この要素の XPath 式を次に示します。<br/><br/>  `/GetAttachment/AttachmentShape` <br/> |
   
## <a name="text-value"></a>テキスト値

**Bodytype**要素に使用できる値を次の表に示します。 
  
|**値**|**説明**|
|:-----|:-----|
|高  <br/> |応答によって、本文の中で最も豊富な利用可能なコンテンツが返されます。 これは、コンテンツがテキストであるか HTML であるかにかかわらず、不明な場合に便利です。<br/><br/> 保存された本文がプレーンテキストの場合、返される本文はテキストになります。 それ以外の場合、保存された本文が HTML または RTF 形式の場合、応答は HTML を返します。<br/><br/> これは既定の値です。  <br/> |
|HTML  <br/> |応答は、アイテムの本文を HTML として返します。  <br/> |
|テキスト  <br/> |応答は、アイテムの本文をプレーンテキストとして返します。  <br/> |
   
## <a name="remarks"></a>注釈

応答で返される本文の種類を特定するには、 [body](body.md)要素の**bodytype**属性をチェックします。 **Bodytype**属性は、本文を HTML またはテキストのいずれかとして識別します。 
  
この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="example"></a>例

次の要求の例は、 **Bodytype**要素が使用されている場所を示しています。 
  
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

Id 属性は読みやすくするために短縮されています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   

