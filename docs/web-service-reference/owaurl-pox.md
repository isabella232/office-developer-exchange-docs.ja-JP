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
description: OWAUrl 要素には、Outlook Web Access をホストするクライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行している特定のコンピューターにアクセスするために使用される URL と認証スキーマが記述されています。
ms.openlocfilehash: c0728af063cfbf1353eb7d3b81f5fcfe8b398f7d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457264"
---
# <a name="owaurl-pox"></a>OWAUrl (POX)

**Owaurl**要素には、Outlook Web access をホストするクライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行している特定のコンピューターにアクセスするために使用される URL と認証スキーマが記述されています。 
  
[自動検出 (POX)](autodiscover-pox.md)
  
[応答 (POX)](response-pox.md)
  
[アカウント (POX)](account-pox.md)
  
[プロトコル (POX)](protocol-pox.md)
  
[Internal (POX)](internal-pox.md)
  
[OWAUrl (POX)](owaurl-pox.md)
  
```xml
<OWAUrl AuthenticationMethod=""/>
```

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**AuthenticationMethod** <br/> |Outlook Web Access にアクセスするための認証方法について説明します。  <br/> |
   
#### <a name="authenticationmethod-attribute"></a>AuthenticationMethod 属性

|**値**|**説明**|
|:-----|:-----|
|WindowsIntegrated  <br/> |統合 Windows 認証。  <br/> |
|FBA  <br/> |フォームベース認証。  <br/> |
|NTLM  <br/> |NTLM 認証。  <br/> |
|Digest  <br/> |ダイジェスト認証。  <br/> |
|基本  <br/> |基本認証。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[Internal (POX)](internal-pox.md) <br/> |クライアントがファイアウォールの内側にいる場合に接続できる Outlook Web Access Url のコレクションが含まれています。  <br/> |
   
## <a name="text-value"></a>テキスト値

Text 値は、クライアントアクセスサーバー上の Outlook Web Access サービスの URL を表します。
  
## <a name="see-also"></a>関連項目



[Exchange の POX 自動検出 XML 要素](pox-autodiscover-xml-elements-for-exchange.md)

