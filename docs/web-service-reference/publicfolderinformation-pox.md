---
title: PublicFolderInformation (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: a221aa9e-b4ac-4ec5-aa42-7e2a69e8eaa6
description: PublicFolderInformation 要素には、クライアントが自動検出要求を送信してユーザーのパブリックフォルダー情報を検出するために使用できる情報が含まれています。
ms.openlocfilehash: e044a1feddfaeb4eb93c289c617dde9adc66f332
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457719"
---
# <a name="publicfolderinformation-pox"></a>PublicFolderInformation (POX)

**Publicfolderinformation**要素には、クライアントが自動検出要求を送信してユーザーのパブリックフォルダー情報を検出するために使用できる情報が含まれています。 
  
[自動検出 (POX)](autodiscover-pox.md)
  
[応答 (POX)](response-pox.md)
  
[アカウント (POX)](account-pox.md)
  
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
|[SmtpAddress (POX)](smtpaddress-pox.md) <br/> |ユーザー用に構成されたパブリックフォルダーメッセージストアに割り当てられている SMTP アドレスが含まれます。 この SMTP アドレスは、自動検出要求の[EMailAddress (POX)](emailaddress-pox.md)要素で、パブリックフォルダーの設定を検出するために使用できます。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[アカウント (POX)](account-pox.md) <br/> |ユーザーのアカウント設定を指定します。  <br/> |
   
## <a name="remarks"></a>注釈

**Publicfolderinformation**要素は、 **Account**要素のオプションの子要素です。 
  
## <a name="see-also"></a>関連項目



[Exchange の POX 自動検出 XML 要素](pox-autodiscover-xml-elements-for-exchange.md)

