---
title: SerializedSecurityContext
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SerializedSecurityContext
api_type:
- schema
ms.assetid: a02c4fc1-ed1a-40d9-a18e-6cfdae21a690
description: SerializedSecurityContext 要素は、サーバー間認証でトークンをシリアル化するための簡易オブジェクトアクセスプロトコル (SOAP) ヘッダーで使用されます。 トークンのシリアル化はサポートされていません。
ms.openlocfilehash: 58fea1c7f613315d59e81935561f92f318afc769
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462053"
---
# <a name="serializedsecuritycontext"></a>SerializedSecurityContext

**SerializedSecurityContext**要素は、サーバー間認証でトークンをシリアル化するための簡易オブジェクトアクセスプロトコル (SOAP) ヘッダーで使用されます。 トークンのシリアル化はサポートされていません。 
  
```xml
<SerializedSecurityContext>
   <UserSid/>
   <GroupSids/>
   <RestrictedGroupSids/>
   <PrimarySmtpAddress/>
</SerializedSecurityContext>
```

 **SerializedSecurityContextType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[UserSid](usersid.md) <br/> |シリアル化されたセキュリティコンテキストの SOAP ヘッダー内のユーザーセキュリティ識別子のセキュリティ記述子定義言語 (SDDL) 形式を表します。  <br/> |
|[GroupSids](groupsids.md) <br/> |Active Directory ディレクトリサービスグループオブジェクトのセキュリティ識別子のコレクションを表します。  <br/> |
|[RestrictedGroupSids](restrictedgroupsids.md) <br/> |制限されたグループのグループセキュリティ識別子と属性を表します。  <br/> |
|[PrimarySmtpAddress](primarysmtpaddress.md) <br/> |サーバー間の認証に使用されるアカウントのプライマリ簡易メール転送プロトコル (SMTP) アドレスを表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバー (CAS) の役割がインストールされています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)


[EWS でのサーバー間認証](https://msdn.microsoft.com/library/f1610a20-672d-448b-8c00-5b0fbcaf31cb%28Office.15%29.aspx)

