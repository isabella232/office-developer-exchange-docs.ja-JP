---
title: Getnonindexableitem、Response
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 6cf2aea3-c6f7-4cad-a45d-2daffeece4b6
description: GetNonIndexableItemDetails Response 要素は、GetNonIndexableItemDetails 要求への応答を指定します。
ms.openlocfilehash: 7563a772e04f72c50ddfea0a69fa511d2a538b8e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455619"
---
# <a name="getnonindexableitemdetailsresponse"></a>Getnonindexableitem、Response

**Getnonindexableitemdetails response**要素は、 **getnonindexableitemdetails**要求への応答を指定します。 
  
```XML
<GetNonIndexableItemDetailsResponse>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <NonIndexableItemDetailsResult/>
</GetNonIndexableItemDetailsResponse>
```

 **Getnonindexableitem/[Responsemessagetype]**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

[Messagetext](messagetext.md)  | 応答[Secmode](responsecode.md)  | [DescriptiveLinkKey](descriptivelinkkey.md)  | [MessageXml](messagexml.md)  | [Nonindexableitemの取得結果](nonindexableitemdetailsresult.md)
  
### <a name="parent-elements"></a>親要素

[ResponseMessages](responsemessages.md)
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空にすることができます。  <br/> |false  <br/> |
   

