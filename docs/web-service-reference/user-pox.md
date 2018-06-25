---
title: ユーザー (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 7c42b516-77f6-4aee-99d8-b866d82d793a
description: ユーザーの要素は、ユーザー固有の情報を提供します。
ms.openlocfilehash: 3f90ff0cc00170170c7304f2a19fe1d7abd9d1bc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19839920"
---
# <a name="user-pox"></a>ユーザー (POX)

**ユーザー**の要素は、ユーザー固有の情報を提供します。 
  
[(POX) を自動検出](autodiscover-pox.md)
  
[応答 (POX)](response-pox.md)
  
[ユーザー (POX)](user-pox.md)
  
```xml
<User>
   <DisplayName/>
   <LegacyDN/>
   <DeploymentId/>
   <AutoDiscoverSMTPAddress/>
</User>
```

## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[表示名 (文字列)](displayname-string.md) <br/> |ユーザーの表示名を表します。  <br/> |
|[LegacyDN (POX)](legacydn-pox.md) <br/> |従来の識別名によって、ユーザーのメールボックスを識別します。  <br/> |
|[DeploymentId (POX)](deploymentid-pox.md) <br/> |Exchange フォレストを一意に識別します。  <br/> |
|[AutoDiscoverSMTPAddress (POX)](autodiscoversmtpaddress-pox.md) <br/> |自動検出プロセスで使用されるユーザーの SMTP アドレスが含まれています。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[応答 (POX)](response-pox.md) <br/> |自動検出サービスからの応答が含まれています。  <br/> |
   
## <a name="remarks"></a>備考

自動検出の要求と応答は、UTF-8 エンコードである必要があります。
  
## <a name="see-also"></a>関連項目



[交換の POX の自動検出の XML 要素](pox-autodiscover-xml-elements-for-exchange.md)

