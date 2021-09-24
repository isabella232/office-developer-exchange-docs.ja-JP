---
title: EcpUrl-tmHiding (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
ms.assetid: 9b9ae15b-3ac1-45ac-85ba-38c7231fe508
description: EcpUrl-tmHiding 要素は、サイト メールボックスからユーザーを登録解除するために使用できる URL を生成するために、EcpUrl (POX) 要素の値と組み合わせ可能な部分 URL を指定します。
ms.openlocfilehash: d8e8ced554b96f1a0cd554d3d601970d5f47019b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59514734"
---
# <a name="ecpurl-tmhiding-pox"></a>EcpUrl-tmHiding (POX)

**EcpUrl-tmHiding** 要素は、サイト メールボックスからユーザーを登録解除するために使用できる URL を生成するために [、EcpUrl (POX)](ecpurl-pox.md)要素の値と組み合わせ可能な部分 URL を指定します。 
  
[AutoDiscover (POX)](autodiscover-pox.md)
  
[Response (POX)](response-pox.md)
  
[Account (POX)](account-pox.md)
  
[Protocol (POX)](protocol-pox.md)
  
[EcpUrl-tmHiding (POX)](ecpurl-tmhiding-pox.md)
  
```XML
<EcpUrl-tmHiding/>
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

テキスト値は [、EcpUrl (POX)](ecpurl-pox.md) 要素の値と組み合わせてサイト メールボックスからユーザーを登録解除するために使用できる URL を生成できる部分的な URL を表します。 **EcpUrl-tmHiding** 要素の値には、次の表に示すように、クライアントによって置き換わる '<' および '>' 文字に含まれるパラメーターが含まれます。 
  
|**パラメーター**|**で置き換える**|
|:-----|:-----|
| _Id_ <br/> |サイト メールボックスの SMTP 電子メール アドレスまたは X500 識別名。  <br/> |
   
## <a name="remarks"></a>注釈

**EcpUrl-tmHiding 要素** は **、Protocol** 要素の省略可能な子要素です。 
  
## <a name="see-also"></a>関連項目



[POX 自動検出 XML 要素のExchange](pox-autodiscover-xml-elements-for-exchange.md)

