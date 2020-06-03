---
title: CompleteName
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CompleteName
api_type:
- schema
ms.assetid: 22d30d1f-a84d-48bb-ad8f-ce13f8e76604
description: CompleteName 要素は、連絡先の完全な名前を表します。
ms.openlocfilehash: 9b5d2646ec37b41cd88d7de61573bfb4a8746cdf
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527174"
---
# <a name="completename"></a>CompleteName

**CompleteName**要素は、連絡先の完全な名前を表します。 
  
```xml
<CompleteName>
   <Title/>
   <FirstName/>
   <MiddleName/>
   <LastName/>
   <Suffix/>
   <Initials/>
   <FullName/>
   <Nickname/>
   <YomiFirstName/>
   <YomiLastName/>
</CompleteName>
```

 **すべての種類**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[Title](title.md) <br/> |連絡先のタイトルを表します。  <br/> |
|[FirstName](firstname.md) <br/> |連絡先の最初の名前を表します。  <br/> |
|[MiddleName](middlename.md) <br/> |連絡先のミドルネームを表します。  <br/> |
|[LastName](lastname.md) <br/> |連絡先の姓を表します。  <br/> |
|[Suffix](suffix.md) <br/> |連絡先の名前のサフィックスを表します。  <br/> |
|[[頭文字](initials.md)] <br/> |連絡先のイニシャルを表します。  <br/> |
|[FullName](fullname.md) <br/> |連絡先の氏名を表します。  <br/> |
|[ニックネーム](nickname.md) <br/> |連絡先のニックネームを表します。  <br/> |
|[YomiFirstName](yomifirstname.md) <br/> |日本語の最初の名前の検索可能な名前またはふりがなのスペルを表すために日本で使用される名前を表します。  <br/> |
|[YomiLastName](yomilastname.md) <br/> |日本語姓の検索可能な名前またはふりがなのスペルを表すために日本で使用される名前を表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[Contact](contact.md) <br/> |Exchange の連絡先アイテムを表します。  <br/> |
   
## <a name="remarks"></a>注釈

CompleteName プロパティは、[既定](https://docs.microsoft.com/dotnet/api/exchangewebservices.defaultshapenamestype?view=exchange-ews-proxy)の図形の一部です。 Microsoft Exchange Server 2007 の最初のリリースバージョンでは、CompleteName プロパティは[GetItem](getitem-operation.md)操作によって返されますが、 [FindItem 操作](finditem-operation.md)は返されません。 Exchange Server 2007 Service Pack 1 (SP1) 以降、 [FindItem 操作](finditem-operation.md)は CompleteName プロパティを[既定](https://docs.microsoft.com/dotnet/api/exchangewebservices.defaultshapenamestype?view=exchange-ews-proxy)の図形でも返します。 この変更はスキーマには影響しません。 
  
この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空にすることができます。  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目

- [すべての種類](https://msdn.microsoft.com/library/ExchangeWebServices.CompleteNameType.aspx)
- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)
- [連絡先の作成 (Exchange Web サービス)](https://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)

