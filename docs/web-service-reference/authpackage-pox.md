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
description: AuthPackage 要素は、メールボックス サーバーの役割がインストールされている Exchange サーバーに対して認証するときに使用される認証スキームを指定します。
ms.openlocfilehash: 120ec00ac82166ae2002a8fbac0edf9a1e23afc7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759468"
---
# <a name="authpackage-pox"></a>AuthPackage (POX)

**AuthPackage**要素は、メールボックス サーバーの役割がインストールされている Exchange サーバーに対して認証するときに使用される認証スキームを指定します。 
  
- [(POX) を自動検出](autodiscover-pox.md)
  
- [応答 (POX)](response-pox.md)
  
- [アカウント (POX)](account-pox.md)
  
- [プロトコル (POX)](protocol-pox.md)
  
- [AuthPackage (POX)](authpackage-pox.md)
  
```xml
<AuthPackage>basic or kerb or kerbntlm or ntlm or certificate or negotiate or nego2</AuthPackage>
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
|[プロトコル (POX)](protocol-pox.md) <br/> |クライアント アクセス サーバーにクライアントを接続するための仕様が含まれています。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は、メールボックス サーバーに対して認証するときに使用されている認証スキームを指定します。 指定可能な値は次のいずれかです。
  
- 基本的な
- kerb
- kerbntlm
- ntlm
- 証明書
- 交渉
- nego2
    
## <a name="remarks"></a>備考

**AuthPackage**要素は、[型 (POX)](type-pox.md)要素に EXCH または EXPR のテキスト値が設定されている場合にのみ使用されます。 
  
### <a name="version-differences"></a>バージョンの相違点

Office 365、Exchange Online では、および設置型バージョンの Exchange から始まる値をビルド 15.00.0995.014 の戻り値「交渉」のネゴシエート認証を使用するサーバーが構成されているクライアントには、 [X-ClientCanHandle](pox-autodiscover-request-for-exchange.md)ヘッダーが含まれて 場合にのみです"Negotiate"が含まれています。 
  
## <a name="see-also"></a>関連項目

- [交換の POX の自動検出の XML 要素](pox-autodiscover-xml-elements-for-exchange.md)

