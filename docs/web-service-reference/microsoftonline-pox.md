---
title: Microsoft Online (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 0b88f02a-9c50-44b3-841b-560b24e37af5
description: Microsoft Office Online 要素には、ユーザーのメールボックスが Office 365 の一部として Exchange Online または Exchange Online でホストされているかどうかを示す値が含まれています。
ms.openlocfilehash: f3144a673a4c98aad821e21c562141b0ae00f426
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467985"
---
# <a name="microsoftonline-pox"></a>Microsoft Online (POX)

**Microsoft Office online**要素には、ユーザーのメールボックスが Office 365 の一部として exchange online または exchange online でホストされているかどうかを示す値が含まれています。 
  
[自動検出 (POX)](autodiscover-pox.md)
  
[応答 (POX)](response-pox.md)
  
[アカウント (POX)](account-pox.md)
  
[Microsoft Online (POX)](microsoftonline-pox.md)
  
```XML
<MicrosoftOnline/>
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
|[アカウント (POX)](account-pox.md) <br/> |ユーザーのアカウント設定を指定します。または、エラー応答を含みます。  <br/> |
   
## <a name="remarks"></a>注釈

テキスト値は、ユーザーのメールボックスが Exchange Online でホストされているかどうかを示します。 この値は、ユーザーのメールボックスが Exchange Online でホストされている場合は**true**です。それ以外の場合は**false**。
  
## <a name="see-also"></a>関連項目



[Exchange の POX 自動検出 XML 要素](pox-autodiscover-xml-elements-for-exchange.md)

