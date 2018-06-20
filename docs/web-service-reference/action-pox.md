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
description: Action 要素では、ユーザーの構成情報を取得する別の自動検出要求が必要かどうかを決定するために使用される情報を提供します。
ms.openlocfilehash: 118bb59f2c929e3c74683dbf3f073da34d67a3e7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760441"
---
# <a name="action-pox"></a>アクション (POX)

**Action**要素では、ユーザーの構成情報を取得する別の自動検出要求が必要かどうかを決定するために使用される情報を提供します。 
  
- [(POX) を自動検出](autodiscover-pox.md)
  
- [応答 (POX)](response-pox.md)
  
- [アカウント (POX)](account-pox.md)
  
- [アクション (POX)](action-pox.md)
  
```xml
<Action>redirectUrl or redirectAddr or settings</Action>
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
|[アカウント (POX)](account-pox.md) <br/> |ユーザーのアカウントの設定を指定します。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は、別の自動検出要求がユーザーの構成情報を取得する必要があるかどうかを表します。 次の表は、可能な値を一覧します。
  
|**値**|**説明**|
|:-----|:-----|
|redirectUrl  <br/> |この値を指定する場合、 [RedirectUrl (POX)](redirecturl-pox.md)要素はそれ以降の自動検出の要求で使用するクライアント アクセス サーバーの URL を指定します。 クライアント アプリケーションでは、10 リダイレクト後のリダイレクトを停止する必要があります。  <br/> |
|redirectAddr  <br/> |この値を指定する場合、 [RedirectAddr (POX)](redirectaddr-pox.md)要素は後続の自動検出要求に使用する電子メール アドレスを指定します。  <br/> |
|settings  <br/> |この値を指定する場合、自動検出の応答には、アカウントを構成するために使用する設定が含まれています。 [プロトコル (POX)](protocol-pox.md)要素にほとんどの設定が存在します。  <br/> |
   
## <a name="see-also"></a>関連項目

- [交換の POX の自動検出の XML 要素](pox-autodiscover-xml-elements-for-exchange.md)

