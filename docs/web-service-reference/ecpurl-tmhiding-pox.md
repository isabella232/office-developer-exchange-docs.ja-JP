---
title: EcpUrl-tmHiding 表示 (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 9b9ae15b-3ac1-45ac-85ba-38c7231fe508
description: EcpUrl 非表示要素は、EcpUrl (POX) 要素の値と組み合わせて、サイトメールボックスからユーザーの登録を解除するために使用できる URL を生成できる url の一部を指定します。
ms.openlocfilehash: 68b949db8b8d98caddbac3b9f96c5d5e55b104b7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463532"
---
# <a name="ecpurl-tmhiding-pox"></a>EcpUrl-tmHiding 表示 (POX)

**EcpUrl 非表示**要素は、 [EcpUrl (POX)](ecpurl-pox.md)要素の値と組み合わせて、サイトメールボックスからユーザーの登録を解除するために使用できる url を生成できる url の一部を指定します。 
  
[自動検出 (POX)](autodiscover-pox.md)
  
[応答 (POX)](response-pox.md)
  
[アカウント (POX)](account-pox.md)
  
[プロトコル (POX)](protocol-pox.md)
  
[EcpUrl-tmHiding 表示 (POX)](ecpurl-tmhiding-pox.md)
  
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
|[プロトコル (POX)](protocol-pox.md) <br/> |クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターにクライアントを接続するための仕様が含まれています。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は、 [EcpUrl (POX)](ecpurl-pox.md)要素の値と組み合わせて、サイトメールボックスからユーザーの登録を解除するために使用できる url を生成できる url の部分を表します。 **EcpUrl 非表示**要素の値には、次の表に示すように、クライアントによって置き換えられる ' < ' および ' > ' 文字に含まれるパラメーターが含まれています。 
  
|**パラメーター**|**代用**|
|:-----|:-----|
| _Id_ <br/> |サイトメールボックスの SMTP 電子メールアドレスまたは X500 識別名。  <br/> |
   
## <a name="remarks"></a>注釈

**EcpUrl 非表示**要素は、 **Protocol**要素のオプションの子要素です。 
  
## <a name="see-also"></a>関連項目



[Exchange の POX 自動検出 XML 要素](pox-autodiscover-xml-elements-for-exchange.md)

