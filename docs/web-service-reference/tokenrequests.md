---
title: TokenRequests
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: fbab89e9-b41a-44c4-8ad3-d46aa8e56652
description: TokenRequests 要素には、トークン要求の配列が含まれています。
ms.openlocfilehash: 01d847d7d496a5bd1d5621a3787d0e3cc6ddd7ff
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19839748"
---
# <a name="tokenrequests"></a>TokenRequests

**TokenRequests**要素には、トークン要求の配列が含まれています。 
  
```XML
<TokenRequests>
   <TokenRequest/>
</TokenRequests>
```

 **NonEmptyArrayOfClientAccessTokenRequestsType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

[TokenRequest](tokenrequest.md)
  
### <a name="parent-elements"></a>親要素

[GetClientAccessToken](getclientaccesstoken.md)
  
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
   

