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
description: ユーザー Id 要素は、代理ユーザー、またはフォルダーのアクセス許可を持つユーザーを識別します。
ms.openlocfilehash: 8e9867f5a8cdd62dd2dae55fbf527595ac14f46d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19839933"
---
# <a name="userid"></a>UserId

**ユーザー Id**要素は、代理ユーザー、またはフォルダーのアクセス許可を持つユーザーを識別します。 
  
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
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[SID](sid.md) <br/> |セキュリティ識別子 (SID) のセキュリティ記述子定義言語 (SDDL) 形式を表します。  <br/> |
|[PrimarySmtpAddress](primarysmtpaddress.md) <br/> |代理人アクセスに使用するアカウントのプライマリ簡易メール転送プロトコル (SMTP) アドレスを表します。  <br/> |
|[表示名 (文字列)](displayname-string.md) <br/> |フォルダー、連絡先、配布リスト、または代理ユーザーの表示名を定義します。  <br/> |
|[DistinguishedUser](distinguisheduser.md) <br/> |代理人アクセスの認証と既定のユーザー アカウントを識別します。  <br/> |
|[ExternalUserIdentity](externaluseridentity.md) <br/> |フォルダーのアクセス許可を持つ外部ユーザー、外部の代理人のユーザーを識別します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[DelegateUser](delegateuser.md) <br/> |1 つのデリゲートを追加するメールボックスの更新を識別します。  <br/> |
|[Permission](permission.md) <br/> |フォルダーにユーザーが持つアクセス権を定義します。  <br/> |
|[CalendarPermission](calendarpermission.md) <br/> |予定表フォルダーにユーザーが持つアクセス権を定義します。  <br/> |
|[ユーザー Id](userids.md) <br/> |取得またはプリンシパルのメールボックスから削除する代理人のユーザーの配列が含まれています。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>備考

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



[AddDelegate 操作](adddelegate-operation.md)
  
[UpdateDelegate 操作](updatedelegate-operation.md)


- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)


[デリゲートを追加します。](http://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

