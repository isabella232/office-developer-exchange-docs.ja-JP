---
title: CompleteName
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- CompleteName
api_type:
- schema
ms.assetid: 22d30d1f-a84d-48bb-ad8f-ce13f8e76604
description: CompleteName 要素は、連絡先の完全な名前を表します。
ms.openlocfilehash: 873d372657089d21e86025cdf7812659ac505491
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59543556"
---
# <a name="completename"></a>CompleteName

**CompleteName 要素** は、連絡先の完全な名前を表します。 
  
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

 **CompleteNameType**
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
|[LastName](lastname.md) <br/> |連絡先の最後の名前を表します。  <br/> |
|[Suffix](suffix.md) <br/> |連絡先の名前のサフィックスを表します。  <br/> |
|[[頭文字](initials.md)] <br/> |連絡先のイニシャルを表します。  <br/> |
|[FullName](fullname.md) <br/> |連絡先の完全な名前を表します。  <br/> |
|[ニックネーム](nickname.md) <br/> |連絡先のニックネームを表します。  <br/> |
|[YomiFirstName](yomifirstname.md) <br/> |日本語のファースト ネームの検索可能なスペルまたは電話のスペルに対して日本で使用される名前を表します。  <br/> |
|[YomiLastName](yomilastname.md) <br/> |日本語の名字の検索可能なスペルまたは電話のスペルに対して日本で使用される名前を表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[Contact](contact.md) <br/> |連絡先アイテムExchangeを表します。  <br/> |
   
## <a name="remarks"></a>注釈

CompleteName プロパティは、既定の図形 [の一部](https://docs.microsoft.com/dotnet/api/exchangewebservices.defaultshapenamestype?view=exchange-ews-proxy) です。 2007 年の最初のリリース バージョンでは Microsoft Exchange Server、CompleteName プロパティは[GetItem](getitem-operation.md)操作によって返されますが[、FindItem 操作は返されません](finditem-operation.md)。 FindItem Exchange Server 2007 Service Pack 1 (SP1) から始まると、[既定](finditem-operation.md)の図形を持つ CompleteName プロパティも[返](https://docs.microsoft.com/dotnet/api/exchangewebservices.defaultshapenamestype?view=exchange-ews-proxy)されます。 この変更はスキーマには影響を与えかねない。 
  
この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている MicrosoftExchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空の場合  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目

- [CompleteNameType](https://msdn.microsoft.com/library/ExchangeWebServices.CompleteNameType.aspx)
- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)
- [連絡先の作成 (Exchange Web サービス)](https://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)

