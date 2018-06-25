---
title: (POX) を EcpUrl 発行
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: a51189db-f6e5-428d-833d-65a209204a5b
description: EcpUrl 発行要素では、メールが有効なユーザーの設定を公開する予定表にアクセスするために使用する URL を生成する EcpUrl (POX) 要素の値と組み合わせて使用できますが、部分的な URL を指定します。
ms.openlocfilehash: 82f55be3ce529f6e57db5ffe18bbdea609b13595
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760185"
---
# <a name="ecpurl-publish-pox"></a>(POX) を EcpUrl 発行

**EcpUrl 発行**要素では、メールが有効なユーザーの設定を公開する予定表にアクセスするために使用する URL を生成する[EcpUrl (POX)](ecpurl-pox.md)要素の値と組み合わせて使用できますが、部分的な URL を指定します。 
  
[(POX) を自動検出](autodiscover-pox.md)
  
[応答 (POX)](response-pox.md)
  
[アカウント (POX)](account-pox.md)
  
[プロトコル (POX)](protocol-pox.md)
  
[(POX) を EcpUrl 発行](ecpurl-publish-pox.md)
  
```XML
<EcpUrl-publish/>
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
|[プロトコル (POX)](protocol-pox.md) <br/> |クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターにクライアントを接続するための仕様が含まれています。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は、ユーザーの予定表の公開設定にアクセスするために使用できる URL を生成する[EcpUrl (POX)](ecpurl-pox.md)要素の値と組み合わせて使用できますが、部分的な URL を表します。 
  
## <a name="remarks"></a>備考

**EcpUrl 発行**要素は、**プロトコル**要素の省略可能な子要素です。 
  
## <a name="see-also"></a>関連項目



[交換の POX の自動検出の XML 要素](pox-autodiscover-xml-elements-for-exchange.md)

