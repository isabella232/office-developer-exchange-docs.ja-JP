---
title: アクション (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: a3462c6b-453c-462a-830d-f29ee4a2babb
description: Action 要素は、ユーザー構成情報を返すために別の自動検出要求が必要かどうかを判断するために使用される情報を提供します。
ms.openlocfilehash: f6d542b908948d09020b850b60ca1bdb025dd342
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529694"
---
# <a name="action-pox"></a>アクション (POX)

**Action**要素は、ユーザー構成情報を返すために別の自動検出要求が必要かどうかを判断するために使用される情報を提供します。 
  
- [自動検出 (POX)](autodiscover-pox.md)
  
- [応答 (POX)](response-pox.md)
  
- [アカウント (POX)](account-pox.md)
  
- [アクション (POX)](action-pox.md)
  
```xml
<Action>redirectUrl or redirectAddr or settings</Action>
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
|[アカウント (POX)](account-pox.md) <br/> |ユーザーのアカウント設定を指定します。  <br/> |
   
## <a name="text-value"></a>テキスト値

Text 値は、ユーザーの構成情報を取得するために別の自動検出要求が必要かどうかを表します。 次の表に、使用可能な値を示します。
  
|**値**|**説明**|
|:-----|:-----|
|redirectUrl  <br/> |この値が指定されている場合、 [Redirecturl (POX)](redirecturl-pox.md)要素は、以降の自動検出要求で使用されるクライアントアクセスサーバーの URL を指定します。 クライアントアプリケーションは、10回リダイレクトした後にリダイレクトを停止する必要があります。  <br/> |
|redirectAddr  <br/> |この値が指定されている場合、 [Redirectaddr (POX)](redirectaddr-pox.md)要素は、以降の自動検出要求に使用する電子メールアドレスを指定します。  <br/> |
|設定  <br/> |この値が指定されている場合、自動検出応答には、アカウントの構成に使用される設定が含まれます。 ほとんどの設定は[Protocol (POX)](protocol-pox.md)要素にあります。  <br/> |
   
## <a name="see-also"></a>関連項目

- [Exchange の POX 自動検出 XML 要素](pox-autodiscover-xml-elements-for-exchange.md)

