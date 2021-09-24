---
title: PublicFolderInformation (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
ms.assetid: a221aa9e-b4ac-4ec5-aa42-7e2a69e8eaa6
description: PublicFolderInformation 要素には、クライアントが自動検出要求を送信してユーザーのパブリック フォルダー情報を検出するために使用できる情報が含まれている。
ms.openlocfilehash: d77ea350f05c5d6137d3b67cfd49119bf9590e53
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59540623"
---
# <a name="publicfolderinformation-pox"></a>PublicFolderInformation (POX)

**PublicFolderInformation** 要素には、クライアントが自動検出要求を送信してユーザーのパブリック フォルダー情報を検出するために使用できる情報が含まれている。 
  
[AutoDiscover (POX)](autodiscover-pox.md)
  
[Response (POX)](response-pox.md)
  
[Account (POX)](account-pox.md)
  
[PublicFolderInformation (POX)](publicfolderinformation-pox.md)
  
```XML
<PublicFolderInformation>
   <SmtpAddress/>
</PublicFolderInformation>
```

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[SmtpAddress (POX)](smtpaddress-pox.md) <br/> |ユーザー用に構成されたパブリック フォルダー メッセージ ストアに割り当てられた SMTP アドレスを格納します。 この SMTP アドレスは、自動検出要求の [EMailAddress (POX)](emailaddress-pox.md) 要素でパブリック フォルダー設定を検出するために使用できます。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[Account (POX)](account-pox.md) <br/> |ユーザーのアカウント設定を指定します。  <br/> |
   
## <a name="remarks"></a>注釈

**PublicFolderInformation 要素は****、Account** 要素の省略可能な子要素です。 
  
## <a name="see-also"></a>関連項目



[POX 自動検出 XML 要素のExchange](pox-autodiscover-xml-elements-for-exchange.md)

