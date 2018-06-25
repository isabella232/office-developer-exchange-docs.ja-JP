---
title: EmwsUrl (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: cad0fa91-8d75-4dde-a484-518c837ae063
description: EmwsUrl 要素は、メールが有効なユーザーの Exchange Web サービス (EWS) の最適なエンドポイントのインスタンスの URL を指定します。
ms.openlocfilehash: d8905d098c9978c3413f67e9a1b2443a52fb0d1f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760270"
---
# <a name="emwsurl-pox"></a>EmwsUrl (POX)

**EmwsUrl**要素は、メールが有効なユーザーの Exchange Web サービス (EWS) の最適なエンドポイントのインスタンスの URL を指定します。 
  
- [(POX) を自動検出](autodiscover-pox.md) 
- [応答 (POX)](response-pox.md) 
- [アカウント (POX)](account-pox.md) 
- [プロトコル (POX)](protocol-pox.md) 
- [EmwsUrl (POX)](emwsurl-pox.md)
  
```XML
<EmwsUrl/>
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

テキスト値は、ユーザーの EWS のエンドポイントの URL を表します。 [EwsUrl (POX)](ewsurl-pox.md)の要素と同じであります。 
  
## <a name="remarks"></a>備考

**EmwsUrl**要素は、**プロトコル**要素の省略可能な子要素です。 
  
## <a name="see-also"></a>関連項目

- [交換の POX の自動検出の XML 要素](pox-autodiscover-xml-elements-for-exchange.md)

