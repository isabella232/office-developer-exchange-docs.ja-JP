---
title: SmtpAddress (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 984ccd97-c337-47b6-ba42-3405a8b55a71
description: SmtpAddress 要素には、ユーザー用に構成するパブリック フォルダーのメッセージ ストアに割り当てられている SMTP アドレスが含まれています。
ms.openlocfilehash: 43ebb328e31cdec11412e80b743d4d4393b7960a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833507"
---
# <a name="smtpaddress-pox"></a>SmtpAddress (POX)

**SmtpAddress**要素には、ユーザー用に構成するパブリック フォルダーのメッセージ ストアに割り当てられている SMTP アドレスが含まれています。 
  
- [(POX) を自動検出](autodiscover-pox.md)
  
- [応答 (POX)](response-pox.md)
  
- [アカウント (POX)](account-pox.md)
  
- [PublicFolderInformation (POX)](publicfolderinformation-pox.md)
  
- [SmtpAddress (POX)](smtpaddress-pox.md)
  
```XML
<SmtpAddress/>
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
|[PublicFolderInformation (POX)](publicfolderinformation-pox.md) <br/> |クライアント ユーザーのパブリック フォルダー情報を検出する自動検出要求の送信に使用できる情報が含まれています。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は、ユーザー用に構成するパブリック フォルダー ストアに割り当てられている SMTP アドレスを表します。 この SMTP アドレスは、パブリック フォルダーの設定を検出する自動検出要求の[EMailAddress (POX)](emailaddress-pox.md)要素で使用できます。 
  
## <a name="remarks"></a>備考

**SmtpAddress**要素は、 **PublicFolderInformation**要素の必須の子要素です。 
  
## <a name="see-also"></a>関連項目

- [交換の POX の自動検出の XML 要素](pox-autodiscover-xml-elements-for-exchange.md)

