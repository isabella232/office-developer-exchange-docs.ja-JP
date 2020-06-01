---
title: SmtpAddress (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 984ccd97-c337-47b6-ba42-3405a8b55a71
description: SmtpAddress 要素には、ユーザー用に構成されたパブリックフォルダーメッセージストアに割り当てられた SMTP アドレスが含まれています。
ms.openlocfilehash: 48703a11fb056967c6c76073c2e928d5f6efa264
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468643"
---
# <a name="smtpaddress-pox"></a>SmtpAddress (POX)

**Smtpaddress**要素には、ユーザー用に構成されたパブリックフォルダーメッセージストアに割り当てられた SMTP アドレスが含まれています。 
  
- [自動検出 (POX)](autodiscover-pox.md)
  
- [応答 (POX)](response-pox.md)
  
- [アカウント (POX)](account-pox.md)
  
- [PublicFolderInformation (POX)](publicfolderinformation-pox.md)
  
- [SmtpAddress (POX)](smtpaddress-pox.md)
  
```XML
<SmtpAddress/>
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
|[PublicFolderInformation (POX)](publicfolderinformation-pox.md) <br/> |クライアントが、ユーザーのパブリックフォルダー情報を検出するために自動検出要求を送信するために使用できる情報が含まれています。  <br/> |
   
## <a name="text-value"></a>テキスト値

Text 値は、ユーザーに対して構成されているパブリックフォルダーストアに割り当てられた SMTP アドレスを表します。 この SMTP アドレスは、自動検出要求の[EMailAddress (POX)](emailaddress-pox.md)要素で、パブリックフォルダーの設定を検出するために使用できます。 
  
## <a name="remarks"></a>注釈

**Smtpaddress**要素は、 **publicfolderinformation**要素の必須の子要素です。 
  
## <a name="see-also"></a>関連項目

- [Exchange の POX 自動検出 XML 要素](pox-autodiscover-xml-elements-for-exchange.md)

