---
title: EcpUrl-tmEditing (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 1fbc2ea9-3f94-441b-ab42-647326bf0021
description: EcpUrl-tmEditing 要素は、既存のサイトメールボックスの編集に使用できる URL を生成するために、(POX) 要素の値と組み合わせることができる部分的な URL を指定します。
ms.openlocfilehash: 5d6c6b8e8f73d113cfde3570065435927ffbae05
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463539"
---
# <a name="ecpurl-tmediting-pox"></a>EcpUrl-tmEditing (POX)

**EcpUrl-tmEditing**要素は、既存のサイトメールボックスの編集に使用できる url を生成するために、 [(POX)](ecpurl-pox.md)要素の値と組み合わせることができる部分的な url を指定します。 
  
[自動検出 (POX)](autodiscover-pox.md)
  
[応答 (POX)](response-pox.md)
  
[アカウント (POX)](account-pox.md)
  
[プロトコル (POX)](protocol-pox.md)
  
[EcpUrl-tmEditing (POX)](ecpurl-tmediting-pox.md)
  
```XML
<EcpUrl-tmEditing/>
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

テキスト値は、 [EcpUrl (POX)](ecpurl-pox.md)要素の値と組み合わせて、既存のサイトメールボックスの編集に使用できる url を生成できる url の部分を表します。 **EcpUrl-tmEditing**要素の値には、次の表に示すように、クライアントによって置き換えられる ' < ' と ' > ' 文字に含まれるパラメーターが含まれています。 
  
|**パラメーター**|**代用**|
|:-----|:-----|
| _Id_ <br/> |サイトメールボックスの SMTP 電子メールアドレスまたは X500 識別名。  <br/> |
   
## <a name="remarks"></a>注釈

**EcpUrl-Tmedioffelement**は、 **Protocol**要素のオプションの子要素です。 
  
## <a name="see-also"></a>関連項目



[Exchange の POX 自動検出 XML 要素](pox-autodiscover-xml-elements-for-exchange.md)

