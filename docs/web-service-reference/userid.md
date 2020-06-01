---
title: UserId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UserId
api_type:
- schema
ms.assetid: 244af9e0-bf3c-46b4-8bfa-9719a1ed3107
description: UserId 要素は、代理ユーザーまたはフォルダーのアクセス許可を持つユーザーを識別します。
ms.openlocfilehash: 68075e335383835ddce9575d85ba5fa945ed305c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455542"
---
# <a name="userid"></a>UserId

**UserId**要素は、代理ユーザーまたはフォルダーのアクセス許可を持つユーザーを識別します。 
  
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
|[PrimarySmtpAddress](primarysmtpaddress.md) <br/> |代理人アクセスに使用するアカウントのプライマリ簡易メール転送プロトコル (SMTP) アドレスを表します。  <br/> |
|[DisplayName (文字列)](displayname-string.md) <br/> |フォルダー、連絡先、配布リスト、または代理人のユーザーの表示名を定義します。  <br/> |
|[DistinguishedUser](distinguisheduser.md) <br/> |代理人アクセスの匿名および既定のユーザーアカウントを識別します。  <br/> |
|[ExternalUserIdentity](externaluseridentity.md) <br/> |外部代理ユーザーまたはフォルダーアクセス許可を持つ外部ユーザーを識別します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[DelegateUser](delegateuser.md) <br/> |メールボックスに追加または更新する単一の代理人を指定します。  <br/> |
|[アクセス許可](permission.md) <br/> |ユーザーがフォルダーに対して持つアクセス許可を定義します。  <br/> |
|[CalendarPermission](calendarpermission.md) <br/> |ユーザーが予定表フォルダーに対して持っているアクセス権を定義します。  <br/> |
|[UserIds](userids.md) <br/> |プリンシパルのメールボックスから取得または削除するデリゲートユーザーの配列を格納します。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



[AddDelegate 操作](adddelegate-operation.md)
  
[UpdateDelegate 操作](updatedelegate-operation.md)


- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)


[代理人の追加](https://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

