---
title: UserId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- UserId
api_type:
- schema
ms.assetid: 244af9e0-bf3c-46b4-8bfa-9719a1ed3107
description: UserId 要素は、代理人ユーザーまたはフォルダー アクセス許可を持つユーザーを識別します。
ms.openlocfilehash: f03914745f8f7f47c64685b3e7c52eefece5ff6d
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59510758"
---
# <a name="userid"></a>UserId

**UserId 要素は**、代理人ユーザーまたはフォルダー アクセス許可を持つユーザーを識別します。 
  
```xml
<UserId>
   <SID/>
   <PrimarySmtpAddress/>
   <DisplayName/>
   <DistinguishedUser/>
   <ExternalUserIdentity/>
</UserId>
```

 **UserIdType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[SID](sid.md) <br/> |セキュリティ識別子 (SID) のセキュリティ記述子定義言語 (SDDL) 形式を表します。  <br/> |
|[PrimarySmtpAddress](primarysmtpaddress.md) <br/> |代理アクセスに使用するアカウントのプライマリ簡易メール転送プロトコル (SMTP) アドレスを表します。  <br/> |
|[DisplayName (string)](displayname-string.md) <br/> |フォルダー、連絡先、配布リスト、または委任ユーザーの表示名を定義します。  <br/> |
|[DistinguishedUser](distinguisheduser.md) <br/> |代理人アクセスの匿名ユーザー アカウントと既定のユーザー アカウントを識別します。  <br/> |
|[ExternalUserIdentity](externaluseridentity.md) <br/> |フォルダー アクセス許可を持つ外部代理人ユーザーまたは外部ユーザーを識別します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[DelegateUser](delegateuser.md) <br/> |メールボックスに追加または更新する 1 つの代理人を識別します。  <br/> |
|[アクセス許可](permission.md) <br/> |ユーザーがフォルダーに対して持つアクセスを定義します。  <br/> |
|[CalendarPermission](calendarpermission.md) <br/> |ユーザーが予定表フォルダーに対して持つアクセスを定義します。  <br/> |
|[UserIds](userids.md) <br/> |プリンシパルのメールボックスから取得または削除する代理人ユーザーの配列を含む。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



[AddDelegate 操作](adddelegate-operation.md)
  
[UpdateDelegate 操作](updatedelegate-operation.md)


- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)


[代理人の追加](https://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

