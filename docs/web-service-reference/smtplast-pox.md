---
title: SMTPLast (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: f1aa8bd9-c6ac-41ac-8d2d-56fb20006005
description: SMTPLast 要素は、簡易メール転送プロトコル (SMTP) サーバーの SMTP サーバーを使用して電子メールを送信する前に電子メールをダウンロードすることが必要かどうかを指定します。
ms.openlocfilehash: 5359f20b33855f4ef48566058bc46bd618e3b2ff
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833505"
---
# <a name="smtplast-pox"></a>SMTPLast (POX)

**SMTPLast**要素は、簡易メール転送プロトコル (SMTP) サーバーの SMTP サーバーを使用して電子メールを送信する前に電子メールをダウンロードすることが必要かどうかを指定します。 
  
- [(POX) を自動検出](autodiscover-pox.md)
  
- [応答 (POX)](response-pox.md)
  
- [アカウント (POX)](account-pox.md)
  
- [プロトコル (POX)](protocol-pox.md)
  
- [SMTPLast (POX)](smtplast-pox.md)
  
```xml
<SMTPLast>on or off</SMTPLast>
```

## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[プロトコル (POX)](protocol-pox.md) <br/> |クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターにクライアントを接続するための仕様が含まれています。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は、SMTP サーバーに電子メールが SMTP サーバーを使用して電子メールを送信する前にダウンロードすることが必要かどうかを指定します。 使用可能な値は、**オン**と**オフを**します。 既定値では**オフ**です。
  
## <a name="see-also"></a>関連項目

- [交換の POX の自動検出の XML 要素](pox-autodiscover-xml-elements-for-exchange.md)

