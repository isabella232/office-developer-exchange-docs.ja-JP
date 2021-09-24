---
title: Action (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: a3462c6b-453c-462a-830d-f29ee4a2babb
description: Action 要素は、ユーザー構成情報を返す際に別の自動検出要求が必要かどうかを判断するために使用される情報を提供します。
ms.openlocfilehash: b1c07fefc6b8033b9b93bd044c04fb07ba289177
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513858"
---
# <a name="action-pox"></a>Action (POX)

**Action 要素** は、ユーザー構成情報を返す際に別の自動検出要求が必要かどうかを判断するために使用される情報を提供します。 
  
- [AutoDiscover (POX)](autodiscover-pox.md)
  
- [Response (POX)](response-pox.md)
  
- [Account (POX)](account-pox.md)
  
- [Action (POX)](action-pox.md)
  
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
|[Account (POX)](account-pox.md) <br/> |ユーザーのアカウント設定を指定します。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は、ユーザーの構成情報を取得するために別の自動検出要求が必要かどうかを表します。 次の表に、使用可能な値を示します。
  
|**値**|**説明**|
|:-----|:-----|
|redirectUrl  <br/> |この値を指定すると [、RedirectUrl (POX)](redirecturl-pox.md) 要素は、後続の自動検出要求で使用するクライアント アクセス サーバーの URL を指定します。 クライアント アプリケーションは、10 回のリダイレクト後にリダイレクトを停止する必要があります。  <br/> |
|redirectAddr  <br/> |この値を指定すると [、RedirectAddr (POX)](redirectaddr-pox.md) 要素は、後続の自動検出要求に使用する電子メール アドレスを指定します。  <br/> |
|設定  <br/> |この値を指定すると、自動検出応答には、アカウントの構成に使用される設定が含まれる。 ほとんどの設定は、プロトコル [(POX) 要素で確認](protocol-pox.md) できます。  <br/> |
   
## <a name="see-also"></a>関連項目

- [POX 自動検出 XML 要素のExchange](pox-autodiscover-xml-elements-for-exchange.md)

