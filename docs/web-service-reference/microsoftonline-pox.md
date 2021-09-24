---
title: MicrosoftOnline (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
ms.assetid: 0b88f02a-9c50-44b3-841b-560b24e37af5
description: MicrosoftOnline 要素には、ユーザーのメールボックスが Exchange Online または Exchange Online の一部としてホストされているかどうかを示す値が含Office 365。
ms.openlocfilehash: fbf230df18ca488babb1523cc7f689923eaeb55b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59510946"
---
# <a name="microsoftonline-pox"></a>MicrosoftOnline (POX)

**MicrosoftOnline 要素** には、ユーザーのメールボックスが Exchange Online または Exchange Online の一部としてホストされているかどうかを示す値が含Office 365。 
  
[AutoDiscover (POX)](autodiscover-pox.md)
  
[Response (POX)](response-pox.md)
  
[Account (POX)](account-pox.md)
  
[MicrosoftOnline (POX)](microsoftonline-pox.md)
  
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
|[Account (POX)](account-pox.md) <br/> |ユーザーのアカウント設定を指定するか、エラー応答を含む。  <br/> |
   
## <a name="remarks"></a>注釈

テキスト値は、ユーザーのメールボックスがユーザーのメールボックスでホストされているかどうかをExchange Online。 この値は **、ユーザー** のメールボックスがホストされている場合は true Exchange Online。それ以外の場合は **false です**。
  
## <a name="see-also"></a>関連項目



[POX 自動検出 XML 要素のExchange](pox-autodiscover-xml-elements-for-exchange.md)

