---
title: TokenRequests
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: fbab89e9-b41a-44c4-8ad3-d46aa8e56652
description: TokenRequests 要素には、トークン要求の配列が含まれます。
ms.openlocfilehash: 262f34bdf0c5c1eaf946d1de7ba656470be99e50
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59527245"
---
# <a name="tokenrequests"></a>TokenRequests

**TokenRequests 要素** には、トークン要求の配列が含まれます。 
  
```XML
<TokenRequests>
   <TokenRequest/>
</TokenRequests>
```

 **NonEmptyArrayOfClientAccessTokenRequestsType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

[TokenRequest](tokenrequest.md)
  
### <a name="parent-elements"></a>親要素

[GetClientAccessToken](getclientaccesstoken.md)
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |messages.xsd  <br/> |
|空の場合  <br/> ||
   

