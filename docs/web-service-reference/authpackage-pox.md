---
title: AuthPackage (POX)
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 709dbe53-6141-41f8-a2b9-a399bae47991
description: AuthPackage 要素は、メールボックスサーバーの役割がインストールされている Exchange サーバーに対する認証時に使用される認証方式を指定します。
ms.openlocfilehash: 5317cf49d354a558417829e1d1b5b67cd6874309
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459105"
---
# <a name="authpackage-pox"></a>AuthPackage (POX)

**Authpackage**要素は、メールボックスサーバーの役割がインストールされている Exchange サーバーに対する認証時に使用される認証方式を指定します。 
  
- [自動検出 (POX)](autodiscover-pox.md)
  
- [応答 (POX)](response-pox.md)
  
- [アカウント (POX)](account-pox.md)
  
- [プロトコル (POX)](protocol-pox.md)
  
- [AuthPackage (POX)](authpackage-pox.md)
  
```xml
<AuthPackage>basic or kerb or kerbntlm or ntlm or certificate or negotiate or nego2</AuthPackage>
```

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[プロトコル (POX)](protocol-pox.md) <br/> |クライアントをクライアントアクセスサーバーに接続するための仕様が含まれています。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は、メールボックスサーバーに対する認証時に使用される認証スキームを指定します。 指定可能な値は次のいずれかです。
  
- 基本的な
- kerb
- kerbntlm
- ntlm
- certificate
- 取り決め
- nego2
    
## <a name="remarks"></a>注釈

**Authpackage**要素は、 [Type (POX)](type-pox.md)要素のテキスト値が EXCH または EXPR の場合にのみ使用されます。 
  
### <a name="version-differences"></a>バージョンの相違点

Office 365、Exchange Online、およびオンプレミスバージョンの Exchange では、サーバーが Negotiate 認証を使用するように構成されており、クライアントに "Negotiate" が含まれる[X ClientCanHandle](pox-autodiscover-request-for-exchange.md)ヘッダーが含まれている場合にのみ、"negotiate" という値を返します。 
  
## <a name="see-also"></a>関連項目

- [Exchange の POX 自動検出 XML 要素](pox-autodiscover-xml-elements-for-exchange.md)

