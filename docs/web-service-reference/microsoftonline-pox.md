---
title: MicrosoftOnline (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 0b88f02a-9c50-44b3-841b-560b24e37af5
description: MicrosoftOnline 要素には、Office 365 の一部としてかどうかユーザーのメールボックスがホストされている Exchange オンラインまたは Exchange Online を示す値が含まれています。
ms.openlocfilehash: b952bfda17b30dcf29812697d225db32718d9781
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832458"
---
# <a name="microsoftonline-pox"></a>MicrosoftOnline (POX)

**MicrosoftOnline**要素には、Office 365 の一部としてかどうかユーザーのメールボックスがホストされている Exchange オンラインまたは Exchange Online を示す値が含まれています。 
  
[(POX) を自動検出](autodiscover-pox.md)
  
[応答 (POX)](response-pox.md)
  
[アカウント (POX)](account-pox.md)
  
[MicrosoftOnline (POX)](microsoftonline-pox.md)
  
```XML
<MicrosoftOnline/>
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
|[アカウント (POX)](account-pox.md) <br/> |ユーザーのアカウントの設定を指定またはエラー応答が含まれています。  <br/> |
   
## <a name="remarks"></a>備考

テキスト値は、Exchange Online でユーザーのメールボックスがホストされているかどうかを示します。 値は、 **true の**場合、ユーザーのメールボックスがホストされている Exchange オンラインです。それ以外の場合、 **false を指定**します。
  
## <a name="see-also"></a>関連項目



[交換の POX の自動検出の XML 要素](pox-autodiscover-xml-elements-for-exchange.md)

