---
title: EmwsUrl (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
ms.assetid: cad0fa91-8d75-4dde-a484-518c837ae063
description: EmwsUrl 要素は、メールが有効なユーザー Exchange Web サービス (EWS) に最適なエンドポイント インスタンスの URL を指定します。
ms.openlocfilehash: d46438f600e226bce95c5e479aca91bfa942535e
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59538176"
---
# <a name="emwsurl-pox"></a>EmwsUrl (POX)

**EmwsUrl** 要素は、メールが有効なユーザー Exchange Web サービス (EWS) に最適なエンドポイント インスタンスの URL を指定します。 
  
- [AutoDiscover (POX)](autodiscover-pox.md) 
- [Response (POX)](response-pox.md) 
- [Account (POX)](account-pox.md) 
- [Protocol (POX)](protocol-pox.md) 
- [EmwsUrl (POX)](emwsurl-pox.md)
  
```XML
<EmwsUrl/>
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

テキスト値は、ユーザーの EWS エンドポイントの URL を表します。 これは [、EwsUrl (POX) 要素と同](ewsurl-pox.md) じです。 
  
## <a name="remarks"></a>注釈

**EmwsUrl** 要素は、Protocol 要素の省略可能な子 **要素** です。 
  
## <a name="see-also"></a>関連項目

- [POX 自動検出 XML 要素のExchange](pox-autodiscover-xml-elements-for-exchange.md)

