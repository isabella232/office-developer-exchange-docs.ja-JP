---
title: UserSid
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- UserSid
api_type:
- schema
ms.assetid: f8a0dcd9-8564-4e35-b307-c5d2761b48d8
description: UserSid 要素は、シリアル化されたセキュリティ コンテキスト SOAP ヘッダー内のユーザー セキュリティ識別子のセキュリティ記述子定義言語 (SDDL) 形式を表します。 トークンのシリアル化はサポートされていません。
ms.openlocfilehash: b32c9fc8347fba07bff57b942adf6510d37ebf2f
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59517351"
---
# <a name="usersid"></a>UserSid

**UserSid 要素は**、シリアル化されたセキュリティ コンテキスト SOAP ヘッダー内のユーザー セキュリティ識別子のセキュリティ記述子定義言語 (SDDL) 形式を表します。 トークンのシリアル化はサポートされていません。 
  
```xml
<UserSid/>
```

 **String**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[SerializedSecurityContext](serializedsecuritycontext.md) <br/> |サーバー間認証でのトークンのシリアル化に SOAP ヘッダーで使用されます。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は、ユーザーのセキュリティ識別子を表します。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている MicrosoftExchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

