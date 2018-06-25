---
title: 名 (EmailAddress)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Name
api_type:
- schema
ms.assetid: c719c55f-d625-4e64-846f-50ac91881443
description: Name 要素は、メールボックス ユーザーの表示名を表します。
ms.openlocfilehash: 6d30f06c3bfd77d2715798349ab084cdf81f21a6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832505"
---
# <a name="name-emailaddress"></a>名 (EmailAddress)

**Name**要素は、メールボックス ユーザーの表示名を表します。 
  
```xml
<Name/>
```

**文字列型 (String)**

## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[電子メール (EmailAddressType)](email-emailaddresstype.md) <br/> |GetUserAvailability クエリのメールボックスのユーザーを表します。  <br/> <br/>以下は、この要素の XPath です。  <br/><br/>  `/GetUserAvailabilityRequest/MailboxDataArray/MailboxData[i]/Email` <br/> |
|[メールボックス (可用性)](mailbox-availability.md) <br/> | SetUserOofSettings または GetUserOofSettings の要求をメールボックスのユーザーを表します。  <br/><br/>  この要素への XPath 式は、次のように。  <br/><br/>  `/GetUserOofSettingsRequest/Mailbox` <br/><br/>  `/SetUserOofSettingsRequest/Mailbox` <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は、この要素が使用される場合に必要です。
  
## <a name="remarks"></a>備考

この要素は、最大で 1 回、[電子メール (EmailAddressType)](email-emailaddresstype.md)の要素で発生します。 この要素は必須ではありません。 
  
> [!NOTE]
> MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。 
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目

- [GetUserAvailability 操作](getuseravailability-operation.md)
- [GetUserAvailabilityRequest](getuseravailabilityrequest.md)
- [ユーザーの状態を取得します。](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

