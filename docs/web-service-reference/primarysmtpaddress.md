---
title: PrimarySmtpAddress
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PrimarySmtpAddress
api_type:
- schema
ms.assetid: eee79904-9412-4e61-b9b8-aff0ce25fade
description: PrimarySmtpAddress 要素は、サーバーからサーバーへの認証に使用するか、代理アクセス権をアカウントのプライマリ簡易メール転送プロトコル (SMTP) アドレスを表します。
ms.openlocfilehash: d33bf22af4ddf6b2f6d8d8d434168264acfaea7c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/15/2018
ms.locfileid: "19832881"
---
# <a name="primarysmtpaddress"></a>PrimarySmtpAddress

**PrimarySmtpAddress**要素は、サーバーからサーバーへの認証に使用するか、代理アクセス権をアカウントのプライマリ簡易メール転送プロトコル (SMTP) アドレスを表します。 
  
```xml
<PrimarySmtpAddress/>
```

 **PrimarySmtpAddressType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ConnectingSID](connectingsid.md) <br/> |ExchangeImpersonation SOAP ヘッダーを使用する際に偽装するアカウントを表します。  <br/> この要素への XPath 式は、次のようにします。  <br/>  `/ExchangeImpersonation/ConnectingSID` <br/> |
|[SerializedSecurityContext](serializedsecuritycontext.md) <br/> |サーバー間認証でトークンのシリアル化を SOAP ヘッダーで使用されます。  <br/> |
|[ユーザー Id](userid.md) <br/> |代理ユーザー、またはフォルダーのアクセス許可を持つユーザーを識別します。  <br/> |
   
## <a name="text-value"></a>テキスト値

SMTP アドレスを表す文字列値は、必要があります。
  
## <a name="remarks"></a>Remarks

Exchange Web サービスでは、メールボックスが、メールボックスのプライマリ SMTP アドレスによって識別することが必要です。 プロキシ アドレスまたは代替アドレスは使用できません。
  
この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
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
  
[代理人アクセスを使用します。](http://msdn.microsoft.com/library/dfd6b4a3-8fd3-47ba-83c0-52465cb5f3f3%28Office.15%29.aspx)

