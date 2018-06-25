---
title: RedirectTarget (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: f8162724-cf9a-4543-a1ad-5846c8b10bfa
description: RedirectTarget (SOAP) の要素には、リダイレクト URL または電子メール アドレスのターゲットが含まれています。
ms.openlocfilehash: 3a8a0c39c6889730c9d17778c6a26f84fcbcd4a7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833019"
---
# <a name="redirecttarget-soap"></a>RedirectTarget (SOAP)

[RedirectTarget (SOAP)](redirecttarget-soap.md)の要素には、リダイレクト URL または電子メール アドレスのターゲットが含まれています。 
  
```XML
<RedirectTarget/>
```

 **string**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[UserResponse (SOAP)](userresponse-soap.md) <br/> |個々 のユーザーの GetUserSettings の要求に対する応答を表します。  <br/> |
|[DomainResponse (SOAP)](domainresponse-soap.md) <br/> |指定したドメインの指定された設定が含まれています。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値には、それ以降の GetUserSettings に使用するリダイレクト URL または電子メール アドレスのターゲットが含まれているか、GetDomainSettings を要求します。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|スキーマ名  <br/> |スキーマの自動検出  <br/> |
|検証ファイル  <br/> |messages.xsd  <br/> |
|空に設定可能  <br/> |True  <br/> |
   

