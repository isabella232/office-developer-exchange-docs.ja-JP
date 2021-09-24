---
title: AuthPackage (POX)
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 709dbe53-6141-41f8-a2b9-a399bae47991
description: AuthPackage 要素は、メールボックス サーバーの役割がインストールされている Exchange サーバーに対して認証するときに使用される認証スキームを指定します。
ms.openlocfilehash: aff4e84cd44d76c2c5a913b6627e1b0c87bab4dc
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513025"
---
# <a name="authpackage-pox"></a>AuthPackage (POX)

**AuthPackage** 要素は、メールボックス サーバーの役割がインストールされている Exchange サーバーに対して認証するときに使用される認証スキームを指定します。 
  
- [AutoDiscover (POX)](autodiscover-pox.md)
  
- [Response (POX)](response-pox.md)
  
- [Account (POX)](account-pox.md)
  
- [Protocol (POX)](protocol-pox.md)
  
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
|[Protocol (POX)](protocol-pox.md) <br/> |クライアントをクライアント アクセス サーバーに接続するための仕様が含まれる。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は、メールボックス サーバーに対する認証時に使用される認証スキームを指定します。 指定可能な値は次のいずれかです。
  
- basic
- kerb
- kerbntlm
- ntlm
- certificate
- ネゴシエート
- nego2
    
## <a name="remarks"></a>注釈

**AuthPackage 要素** は [、Type (POX)](type-pox.md)要素に EXCH または EXPR のテキスト値がある場合にのみ使用されます。 
  
### <a name="version-differences"></a>バージョンの相違点

Office 365、Exchange Online、およびビルド 15.00.0995.014 から始まる Exchange のオンプレミス バージョンは、サーバーがネゴシエート認証を使用するように構成され、クライアントに "Negotiate" を含む[X-ClientCanHandle](pox-autodiscover-request-for-exchange.md)ヘッダーが含まれている場合にのみ、"ネゴシエート" の値を返します。 
  
## <a name="see-also"></a>関連項目

- [POX 自動検出 XML 要素のExchange](pox-autodiscover-xml-elements-for-exchange.md)

