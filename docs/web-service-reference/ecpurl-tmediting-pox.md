---
title: EcpUrl-tmEditing (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
ms.assetid: 1fbc2ea9-3f94-441b-ab42-647326bf0021
description: EcpUrl-tmEditing 要素は、EcpUrl (POX) 要素の値と組み合わせて、既存のサイト メールボックスの編集に使用できる URL を生成できる部分 URL を指定します。
ms.openlocfilehash: e615e8ae09c3a9422f753a71070917a41f40741b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59531093"
---
# <a name="ecpurl-tmediting-pox"></a>EcpUrl-tmEditing (POX)

**EcpUrl-tmEditing** 要素は [、EcpUrl (POX)](ecpurl-pox.md)要素の値と組み合わせて、既存のサイト メールボックスの編集に使用できる URL を生成できる部分 URL を指定します。 
  
[AutoDiscover (POX)](autodiscover-pox.md)
  
[Response (POX)](response-pox.md)
  
[Account (POX)](account-pox.md)
  
[Protocol (POX)](protocol-pox.md)
  
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
|[Protocol (POX)](protocol-pox.md) <br/> |クライアント アクセス サーバーの役割がインストールされているクライアントを実行しているコンピューター Microsoft Exchange Server接続するための仕様が含まれている。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は [、EcpUrl (POX)](ecpurl-pox.md) 要素の値と組み合わせて、既存のサイト メールボックスの編集に使用できる URL を生成できる部分的な URL を表します。 **EcpUrl-tmEditing** 要素の値には、次の表に示すように、クライアントによって置き換わる '<' および '>' 文字内に含まれるパラメーターが含まれます。 
  
|**パラメーター**|**で置き換える**|
|:-----|:-----|
| _Id_ <br/> |サイト メールボックスの SMTP 電子メール アドレスまたは X500 識別名。  <br/> |
   
## <a name="remarks"></a>注釈

**EcpUrl-tmEditing 要素** は **、Protocol** 要素の省略可能な子要素です。 
  
## <a name="see-also"></a>関連項目



[POX 自動検出 XML 要素のExchange](pox-autodiscover-xml-elements-for-exchange.md)

