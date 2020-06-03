---
title: EmailAddresses
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- EmailAddresses
api_type:
- schema
ms.assetid: fd4d773c-f7dc-4a04-9025-e772d7a45fdf
description: EmailAddresses 要素は、連絡先の電子メールアドレスのコレクションを表します。
ms.openlocfilehash: 9d247f6159d621124ecdd9968ee468ed2b4fe84b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456179"
---
# <a name="emailaddresses"></a>EmailAddresses

**Emailaddresses**要素は、連絡先の電子メールアドレスのコレクションを表します。 
  
```xml
<EmailAddresses>
   <Entry/>
</EmailAddresses>
```

 **EmailAddressDictionaryType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[Entry (EmailAddress)](entry-emailaddress.md) <br/> |連絡先の1つの電子メールアドレスを表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[Contact](contact.md) <br/> |Exchange の連絡先アイテムを表します。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空にすることができます。  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目

- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)
- [連絡先の作成 (Exchange Web サービス)](https://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx) 
- [連絡先の更新](https://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx) 
- [連絡先の削除](https://msdn.microsoft.com/library/fcc3dc84-cd3e-455e-a1a7-ae6921c9b588%28Office.15%29.aspx)

