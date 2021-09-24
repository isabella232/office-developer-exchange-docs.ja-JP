---
title: OWAUrl (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 450b86a1-1722-49f5-b541-16c1edc3db7a
description: OWAUrl 要素は、Microsoft Exchange Server Web Access をホストするクライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 200 Outlook 7 を実行している特定のコンピューターにアクセスするために使用される URL と認証スキーマについて説明します。
ms.openlocfilehash: fbd61eb75018c57dada40f5ed7472379d365e752
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59534892"
---
# <a name="owaurl-pox"></a>OWAUrl (POX)

**OWAUrl** 要素は、Outlook Web Access をホストするクライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行している特定のコンピューターにアクセスするために使用される URL と認証スキーマについて説明します。 
  
[AutoDiscover (POX)](autodiscover-pox.md)
  
[Response (POX)](response-pox.md)
  
[Account (POX)](account-pox.md)
  
[Protocol (POX)](protocol-pox.md)
  
[内部 (POX)](internal-pox.md)
  
[OWAUrl (POX)](owaurl-pox.md)
  
```xml
<OWAUrl AuthenticationMethod=""/>
```

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**AuthenticationMethod** <br/> |Web Access にアクセスする認証方法Outlook説明します。  <br/> |
   
#### <a name="authenticationmethod-attribute"></a>AuthenticationMethod 属性

|**値**|**説明**|
|:-----|:-----|
|WindowsIntegrated  <br/> |統合Windows認証。  <br/> |
|FBA  <br/> |フォーム ベースの認証。  <br/> |
|NTLM  <br/> |NTLM 認証。  <br/> |
|Digest  <br/> |ダイジェスト認証。  <br/> |
|基本  <br/> |基本認証。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[内部 (POX)](internal-pox.md) <br/> |クライアントがファイアウォール内Outlook接続できる Web Access URL のコレクションを格納します。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は、クライアント アクセス サーバー上Outlook Web Access サービスの URL を表します。
  
## <a name="see-also"></a>関連項目



[POX 自動検出 XML 要素のExchange](pox-autodiscover-xml-elements-for-exchange.md)

