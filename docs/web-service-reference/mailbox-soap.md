---
title: Mailbox (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 4ad59e5b-4047-4c34-a318-ca06c31d3de8
description: Mailbox 要素には、検出するユーザーの電子メール アドレスが含まれる。
ms.openlocfilehash: 6349a28b7ed97cfaa2bb8ef8f68d93e16d81c377
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59514285"
---
# <a name="mailbox-soap"></a>Mailbox (SOAP)

**Mailbox 要素** には、検出するユーザーの電子メール アドレスが含まれる。 
  
```XML
<Mailbox/>
```

**string**

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[User (SOAP)](user-soap.md) <br/> |1 人のユーザーの ID を表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

Mailbox 要素のテキスト **値** は、検出するユーザーの電子メール アドレスです。 
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|スキーマ名  <br/> |自動検出スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |正解  <br/> |
   
## <a name="see-also"></a>関連項目

- [GetUserSettings 操作 (SOAP)](getusersettings-operation-soap.md)

