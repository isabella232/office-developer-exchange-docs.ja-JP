---
title: MarkAllItemsAsReadResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: e52f56d4-c6a3-458a-8abb-4e0c19d32341
description: MarkAllItemsAsReadResponseMessage 要素は、MarkAllItemsAsRead 要求の応答メッセージを指定します。
ms.openlocfilehash: e1e0ba3748fe12b6c7f54f0acaa5e1f699a4869a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832349"
---
# <a name="markallitemsasreadresponsemessage"></a>MarkAllItemsAsReadResponseMessage

**MarkAllItemsAsReadResponseMessage**要素は、 **MarkAllItemsAsRead**要求の応答メッセージを指定します。 
  
```XML
<MarkAllItemsAsReadResponseMessage>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</MarkAllItemsAsReadResponseMessage>
```

 ****
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

[メッセージ テキスト](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md)
  
### <a name="parent-elements"></a>親要素

[ResponseMessages](responsemessages.md)
  
## <a name="remarks"></a>備考

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |messages.xsd  <br/> |
|空にすることができます。  <br/> ||
   

