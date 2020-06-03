---
title: EmwsUrl (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: cad0fa91-8d75-4dde-a484-518c837ae063
description: EmwsUrl 要素は、メールが有効なユーザーのために、Exchange Web サービス (EWS) の最適なエンドポイントインスタンスの URL を指定します。
ms.openlocfilehash: 19e1078ae8d08513e85d75d87e960a910986f727
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530671"
---
# <a name="emwsurl-pox"></a>EmwsUrl (POX)

**Emwsurl**要素は、メールが有効なユーザーのために、Exchange Web サービス (EWS) の最適なエンドポイントインスタンスの URL を指定します。 
  
- [自動検出 (POX)](autodiscover-pox.md) 
- [応答 (POX)](response-pox.md) 
- [アカウント (POX)](account-pox.md) 
- [プロトコル (POX)](protocol-pox.md) 
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
|[プロトコル (POX)](protocol-pox.md) <br/> |クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターにクライアントを接続するための仕様が含まれています。  <br/> |
   
## <a name="text-value"></a>テキスト値

Text 値は、ユーザーの EWS エンドポイントの URL を表します。 [Ewsurl (POX)](ewsurl-pox.md)要素と同じです。 
  
## <a name="remarks"></a>注釈

**Emwsurl**要素は、 **Protocol**要素のオプションの子要素です。 
  
## <a name="see-also"></a>関連項目

- [Exchange の POX 自動検出 XML 要素](pox-autodiscover-xml-elements-for-exchange.md)

