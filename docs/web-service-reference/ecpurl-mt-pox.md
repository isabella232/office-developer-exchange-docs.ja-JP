---
title: EcpUrl-mt (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
ms.assetid: 5221745b-572c-44a5-afdb-41b58af44971
description: EcpUrl-mt 要素は、メールが有効なユーザーの電子メール メッセージ追跡設定にアクセスするために使用できる URL を生成するために、EcpUrl (POX) 要素の値と組み合わせ可能な部分 URL を指定します。
ms.openlocfilehash: bb0a60f3b3a2d65421164e40537e7514df20e357
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59520816"
---
# <a name="ecpurl-mt-pox"></a>EcpUrl-mt (POX)

**EcpUrl-mt** 要素は、メールが有効なユーザーの電子メール メッセージ追跡設定にアクセスするために使用できる URL を生成するために [、EcpUrl (POX)](ecpurl-pox.md)要素の値と組み合わせ可能な部分 URL を指定します。 
  
[AutoDiscover (POX)](autodiscover-pox.md)
  
[Response (POX)](response-pox.md)
  
[Account (POX)](account-pox.md)
  
[Protocol (POX)](protocol-pox.md)
  
[EcpUrl-mt (POX)](ecpurl-mt-pox.md)
  
```XML
<EcpUrl-mt/>
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

テキスト値は [、EcpUrl (POX)](ecpurl-pox.md) 要素の値と組み合わせて、ユーザーの電子メール追跡設定にアクセスするために使用できる URL を生成できる部分的な URL を表します。 **EcpUrl-mt** 要素の値には、次の表に示すように、クライアントによって置き換わる '<' 文字と '>' 文字に含まれるパラメーターが含まれます。 
  
|**パラメーター**|**で置き換える**|
|:-----|:-----|
| _IsOwa_ <br/> |n  <br/> |
| _MsgID_ <br/> |Message-ID ヘッダーで指定された通り追跡するメッセージのインターネット メッセージ識別子。  <br/> |
| _Mbx_ <br/> |メールボックス所有者の SMTP アドレス。  <br/> |
| _Sender_ <br/> |メッセージの送信者の SMTP アドレス。  <br/> |
   
## <a name="remarks"></a>注釈

**EcpUrl-mt** 要素は **、Protocol** 要素のオプションの子要素です。 
  
## <a name="see-also"></a>関連項目



[POX 自動検出 XML 要素のExchange](pox-autodiscover-xml-elements-for-exchange.md)

