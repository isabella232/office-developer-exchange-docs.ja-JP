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
description: BodyType 要素は、応答の本文のテキストを書式設定する方法を識別します。
ms.openlocfilehash: f8be2e96390b40faa367cf0d34c533accc3b8afb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759537"
---
# <a name="bodytype"></a>BodyType

**BodyType**要素は、応答の本文のテキストを書式設定する方法を識別します。 
  
```xml
<BodyType>Best or HTML or Text</BodyType>
```

**BodyTypeResponseType**

## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ItemShape](itemshape.md) <br/> | GetItem、FindItem、または SyncFolderItems の応答に含めるコンテンツ アイテムのプロパティを識別します。  <br/><br/>この要素への XPath 式は、次のように。<br/><br/>  `/GetItem/ItemShape`<br/><br/>`/FindItem/ItemShape`<br/><br/>`/SyncFolderItems/ItemShape` <br/> |
|[AttachmentShape](attachmentshape.md) <br/> |[GetAttachment](getattachment.md)要求への応答で返されるその他の拡張アイテム プロパティを識別します。  <br/><br/>この要素への XPath 式は、次のようにします。<br/><br/>  `/GetAttachment/AttachmentShape` <br/> |
   
## <a name="text-value"></a>テキスト値

**BodyType**要素の有効な値を次の表に一覧します。 
  
|**値**|**説明**|
|:-----|:-----|
|ベスト  <br/> |応答には、本文テキストの豊富な利用可能なコンテンツが返されます。 これは、コンテンツは、テキストまたは html 形式かどうか不明ではない場合に便利です。<br/><br/> ストアド本文がテキスト形式の場合は、返された本文をテキストになります。 それ以外の場合、応答であっても、ストアドの本文が HTML または rtf 形式のいずれかの形式では場合、HTML が返されます。<br/><br/> 既定値です。  <br/> |
|HTML  <br/> |応答では、アイテムの本文を HTML として返します。  <br/> |
|テキスト型 (Text)  <br/> |応答では、アイテムの本文をプレーン テキストとして返します。  <br/> |
   
## <a name="remarks"></a>備考

[Body](body.md)要素の**BodyType**属性を確認することによって応答で返される本文の種類を識別することができます。 **BodyType**属性は、HTML またはテキストのいずれかとして本体を識別します。 
  
MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。
  
## <a name="example"></a>例

**BodyType**要素が使用されている要求の次の使用例を示しています。 
  
```xml
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetAttachment xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

Id 属性が読みやすさを維持するのには小さすぎます。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   

