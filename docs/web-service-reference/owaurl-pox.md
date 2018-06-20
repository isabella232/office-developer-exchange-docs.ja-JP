---
title: OWAUrl (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 450b86a1-1722-49f5-b541-16c1edc3db7a
description: OWAUrl 要素は、URL を説明し、Microsoft Exchange Server 2007 を実行する特定のコンピューターへのアクセスに使用する認証スキーマには、クライアント アクセス サーバーの役割がインストールされている Outlook Web Access をホストしています。
ms.openlocfilehash: 93d03506e2a74aa1b4ef6d2a49ccbda01cfc1f9a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832673"
---
# <a name="owaurl-pox"></a>OWAUrl (POX)

**OWAUrl**要素は、URL を説明し、Microsoft Exchange Server 2007 を実行する特定のコンピューターへのアクセスに使用する認証スキーマには、クライアント アクセス サーバーの役割がインストールされている Outlook Web Access をホストしています。 
  
[(POX) を自動検出](autodiscover-pox.md)
  
[応答 (POX)](response-pox.md)
  
[アカウント (POX)](account-pox.md)
  
[プロトコル (POX)](protocol-pox.md)
  
[内部 (POX)](internal-pox.md)
  
[OWAUrl (POX)](owaurl-pox.md)
  
```xml
<OWAUrl AuthenticationMethod=""/>
```

## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**AuthenticationMethod** <br/> |Outlook Web Access にアクセスするための認証方法をについて説明します。  <br/> |
   
#### <a name="authenticationmethod-attribute"></a>AuthenticationMethod 属性

|**値**|**説明**|
|:-----|:-----|
|WindowsIntegrated  <br/> |統合 Windows 認証をします。  <br/> |
|FBA  <br/> |フォーム ベースの認証です。  <br/> |
|NTLM  <br/> |NTLM 認証します。  <br/> |
|Digest  <br/> |ダイジェスト認証です。  <br/> |
|基本  <br/> |基本認証。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[内部 (POX)](internal-pox.md) <br/> |ファイアウォールの内側になる場合にクライアントが接続できる Outlook Web アクセス Url のコレクションが含まれています。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は、クライアント アクセス サーバー上の Outlook Web Access サービスの URL を表します。
  
## <a name="see-also"></a>関連項目



[交換の POX の自動検出の XML 要素](pox-autodiscover-xml-elements-for-exchange.md)

