---
title: EcpUrl-ret (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
ms.assetid: 5f090fd2-b0c4-4ca0-a959-1433d73a2069
description: EcpUrl-ret 要素は、メールが有効なユーザーの保持タグ設定にアクセスするために使用できる URL を生成するために EcpUrl (POX) 要素の値と組み合わせ可能な部分 URL を指定します。
ms.openlocfilehash: f65aa9a2fa934fb21e71f51488a28e9f8f043209
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59538297"
---
# <a name="ecpurl-ret-pox"></a>EcpUrl-ret (POX)

**EcpUrl-ret** 要素は、メールが有効なユーザーの保持タグ設定にアクセスするために使用できる URL を生成するために [EcpUrl (POX)](ecpurl-pox.md)要素の値と組み合わせ可能な部分 URL を指定します。 
  
[AutoDiscover (POX)](autodiscover-pox.md)
  
[Response (POX)](response-pox.md)
  
[Account (POX)](account-pox.md)
  
[Protocol (POX)](protocol-pox.md)
  
[EcpUrl-ret (POX)](ecpurl-ret-pox.md)
  
```XML
<EcpUrl-ret/>
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
|[Protocol (POX)](protocol-pox.md) <br/> |クライアント アクセス サーバーの役割がインストールされているクライアントを実行しているコンピューター Microsoft Exchange Server接続するための仕様が含まれている。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は [、EcpUrl (POX)](ecpurl-pox.md) 要素の値と組み合わせて、ユーザーの保持タグ設定にアクセスするために使用できる URL を生成できる部分的な URL を表します。 
  
## <a name="remarks"></a>注釈

**EcpUrl-ret** 要素は **、Protocol** 要素の省略可能な子要素です。 
  
## <a name="see-also"></a>関連項目



[POX 自動検出 XML 要素のExchange](pox-autodiscover-xml-elements-for-exchange.md)

