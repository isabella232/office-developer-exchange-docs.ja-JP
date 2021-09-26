---
title: SmtpAddress (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
ms.assetid: 984ccd97-c337-47b6-ba42-3405a8b55a71
description: SmtpAddress 要素には、ユーザー用に構成されたパブリック フォルダー メッセージ ストアに割り当てられた SMTP アドレスが含まれる。
ms.openlocfilehash: d257b193a3254afceaa72d396a8c2724bb3165c6
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59546988"
---
# <a name="smtpaddress-pox"></a>SmtpAddress (POX)

**SmtpAddress 要素には**、ユーザー用に構成されたパブリック フォルダー メッセージ ストアに割り当てられた SMTP アドレスが含まれる。 
  
- [AutoDiscover (POX)](autodiscover-pox.md)
  
- [Response (POX)](response-pox.md)
  
- [Account (POX)](account-pox.md)
  
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
|[PublicFolderInformation (POX)](publicfolderinformation-pox.md) <br/> |クライアントが自動検出要求を送信して、ユーザーのパブリック フォルダー情報を検出するために使用できる情報が含まれる。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は、ユーザー用に構成されたパブリック フォルダー ストアに割り当てられた SMTP アドレスを表します。 この SMTP アドレスは、自動検出要求の [EMailAddress (POX)](emailaddress-pox.md) 要素でパブリック フォルダー設定を検出するために使用できます。 
  
## <a name="remarks"></a>注釈

**SmtpAddress 要素** は **、PublicFolderInformation** 要素の必須の子要素です。 
  
## <a name="see-also"></a>関連項目

- [POX 自動検出 XML 要素のExchange](pox-autodiscover-xml-elements-for-exchange.md)

