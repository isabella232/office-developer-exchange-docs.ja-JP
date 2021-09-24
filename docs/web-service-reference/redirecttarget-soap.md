---
title: RedirectTarget (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: f8162724-cf9a-4543-a1ad-5846c8b10bfa
description: RedirectTarget (SOAP) 要素には、リダイレクト URL または電子メール アドレスのターゲットが含まれる。
ms.openlocfilehash: 0e09529f62dfde66f1ef05875bb0b0a0886db452
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513543"
---
# <a name="redirecttarget-soap"></a>RedirectTarget (SOAP)

[RedirectTarget (SOAP)](redirecttarget-soap.md)要素には、リダイレクト URL または電子メール アドレスのターゲットが含まれる。 
  
```XML
<RedirectTarget/>
```

 **string**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[UserResponse (SOAP)](userresponse-soap.md) <br/> |個々のユーザーの GetUserSettings 要求に対する応答を表します。  <br/> |
|[DomainResponse (SOAP)](domainresponse-soap.md) <br/> |指定したドメインの要求された設定が含まれる。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値には、後続の GetUserSettings または GetDomainSettings 要求に使用するリダイレクト URL または電子メール アドレスのターゲットが含まれる。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|スキーマ名  <br/> |自動検出スキーマ  <br/> |
|検証ファイル  <br/> |messages.xsd  <br/> |
|空に設定可能  <br/> |はい  <br/> |
   

