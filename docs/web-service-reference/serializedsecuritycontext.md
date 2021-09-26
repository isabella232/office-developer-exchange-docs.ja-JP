---
title: SerializedSecurityContext
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- SerializedSecurityContext
api_type:
- schema
ms.assetid: a02c4fc1-ed1a-40d9-a18e-6cfdae21a690
description: SerializedSecurityContext 要素は、サーバー間Simple Object Access Protocol認証でトークンのシリアル化を行う場合Simple Object Access Protocol (SOAP) ヘッダーで使用されます。 トークンのシリアル化はサポートされていません。
ms.openlocfilehash: 55fe752813fc2d7e3ed5416401ff46b5e00516e3
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59546043"
---
# <a name="serializedsecuritycontext"></a>SerializedSecurityContext

**SerializedSecurityContext** 要素は、サーバー間認証Simple Object Access Protocolトークンのシリアル化のために、SOAP (SOAP) ヘッダーで使用されます。 トークンのシリアル化はサポートされていません。 
  
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
|[UserSid](usersid.md) <br/> |シリアル化されたセキュリティ コンテキスト SOAP ヘッダーのユーザー セキュリティ識別子のセキュリティ記述子定義言語 (SDDL) 形式を表します。  <br/> |
|[GroupSids](groupsids.md) <br/> |Active Directory ディレクトリ サービス グループ オブジェクトのセキュリティ識別子のコレクションを表します。  <br/> |
|[RestrictedGroupSids](restrictedgroupsids.md) <br/> |制限付きグループのグループ セキュリティ識別子と属性を表します。  <br/> |
|[PrimarySmtpAddress](primarysmtpaddress.md) <br/> |サーバー間認証に使用するアカウントのプライマリ簡易メール転送プロトコル (SMTP) アドレスを表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアント アクセス サーバー (CAS) の役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)


[EWS でのサーバー間認証](https://msdn.microsoft.com/library/f1610a20-672d-448b-8c00-5b0fbcaf31cb%28Office.15%29.aspx)

