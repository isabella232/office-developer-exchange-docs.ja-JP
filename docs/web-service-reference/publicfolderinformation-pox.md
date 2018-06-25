---
title: PublicFolderInformation (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: a221aa9e-b4ac-4ec5-aa42-7e2a69e8eaa6
description: PublicFolderInformation 要素には、クライアント ユーザーのパブリック フォルダー情報を検出する自動検出要求の送信に使用できる情報が含まれています。
ms.openlocfilehash: bb4432a664024c3d1ccb17826948cfe7a1b58cdf
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832927"
---
# <a name="publicfolderinformation-pox"></a>PublicFolderInformation (POX)

**PublicFolderInformation**要素には、クライアント ユーザーのパブリック フォルダー情報を検出する自動検出要求の送信に使用できる情報が含まれています。 
  
[(POX) を自動検出](autodiscover-pox.md)
  
[応答 (POX)](response-pox.md)
  
[アカウント (POX)](account-pox.md)
  
[PublicFolderInformation (POX)](publicfolderinformation-pox.md)
  
```XML
<PublicFolderInformation>
   <SmtpAddress/>
</PublicFolderInformation>
```

## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[SmtpAddress (POX)](smtpaddress-pox.md) <br/> |ユーザー用に構成するパブリック フォルダーのメッセージ ストアに割り当てられている SMTP アドレスが含まれています。 この SMTP アドレスは、パブリック フォルダーの設定を検出する自動検出要求の[EMailAddress (POX)](emailaddress-pox.md)要素で使用できます。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[アカウント (POX)](account-pox.md) <br/> |ユーザーのアカウントの設定を指定します。  <br/> |
   
## <a name="remarks"></a>備考

**PublicFolderInformation**要素は、**アカウント**の要素の省略可能な子要素です。 
  
## <a name="see-also"></a>関連項目



[交換の POX の自動検出の XML 要素](pox-autodiscover-xml-elements-for-exchange.md)

