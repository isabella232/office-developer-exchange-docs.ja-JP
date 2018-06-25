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
description: SerializedSecurityContext 要素は、サーバーからサーバーへの認証でトークンのシリアル化に、Simple Object Access Protocol (SOAP) ヘッダーで使用されます。 トークンのシリアル化はサポートされていません。
ms.openlocfilehash: c5590551dc0780d918b05902e4f48fb9d1390b59
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833363"
---
# <a name="serializedsecuritycontext"></a>SerializedSecurityContext

**SerializedSecurityContext**要素は、サーバーからサーバーへの認証でトークンのシリアル化に、Simple Object Access Protocol (SOAP) ヘッダーで使用されます。 トークンのシリアル化はサポートされていません。 
  
```xml
<SerializedSecurityContext>
   <UserSid/>
   <GroupSids/>
   <RestrictedGroupSids/>
   <PrimarySmtpAddress/>
</SerializedSecurityContext>
```

 **SerializedSecurityContextType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[UserSid](usersid.md) <br/> |セキュリティ記述子定義言語 (SDDL) 形式のシリアル化されたセキュリティ コンテキストの SOAP ヘッダーでユーザーのセキュリティ識別子を表します。  <br/> |
|[GroupSids](groupsids.md) <br/> |Active Directory ディレクトリ サービス グループ オブジェクト セキュリティ識別子のコレクションを表します。  <br/> |
|[RestrictedGroupSids](restrictedgroupsids.md) <br/> |グループ セキュリティ識別子および制限されたグループの属性を表します。  <br/> |
|[PrimarySmtpAddress](primarysmtpaddress.md) <br/> |サーバーからサーバーへの認証に使用するアカウントのプライマリ簡易メール転送プロトコル (SMTP) アドレスを表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="remarks"></a>備考

この要素を記述するスキーマは、クライアント アクセス サーバー (CAS) の役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)


[EWS でのサーバーからサーバーへの承認](http://msdn.microsoft.com/library/f1610a20-672d-448b-8c00-5b0fbcaf31cb%28Office.15%29.aspx)

