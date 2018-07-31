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
ms.openlocfilehash: bca6f7e0eb915841673d00b5485da2f0f9794e80
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/28/2018
ms.locfileid: "21354261"
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

 **CompleteNameType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[Title](title.md) <br/> |連絡先のタイトルを表します。  <br/> |
|[FirstName](firstname.md) <br/> |連絡先の名前を表します。  <br/> |
|[MiddleName](middlename.md) <br/> |連絡先のミドル ネームを表します。  <br/> |
|[LastName](lastname.md) <br/> |連絡先の姓を表します。  <br/> |
|[Suffix](suffix.md) <br/> |連絡先の名前にサフィックスを表します。  <br/> |
|[[頭文字]](initials.md) <br/> |連絡先のイニシャルを表します。  <br/> |
|[FullName](fullname.md) <br/> |連絡先の完全名を表します。  <br/> |
|[Nickname](nickname.md) <br/> |連絡先のニックネームを表します。  <br/> |
|[YomiFirstName](yomifirstname.md) <br/> |日本語の姓の検索可能なまたはふりがなのスペル チェックを日本で使用される名前を表します。  <br/> |
|[YomiLastName](yomilastname.md) <br/> |日本語の姓のふりがな、または検索可能なスペルの日本で使用される名前を表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[連絡先](contact.md) <br/> |Exchange の連絡先アイテムを表します。  <br/> |
   
## <a name="remarks"></a>注釈

CompleteName プロパティは、[既定](https://docs.microsoft.com/en-us/dotnet/api/exchangewebservices.defaultshapenamestype?view=exchange-ews-proxy)の図形の一部です。 Microsoft Exchange Server 2007 の最初のリリース バージョン、 [GetItem 操作](getitem-operation.md)が[FindItem 操作](finditem-operation.md)ではなく、CompleteName プロパティが返されます。 Exchange Server 2007 Service Pack 1 (SP1) から始めて、 [FindItem 操作](finditem-operation.md)はまた、[既定](https://docs.microsoft.com/en-us/dotnet/api/exchangewebservices.defaultshapenamestype?view=exchange-ews-proxy)の図形を使用して CompleteName プロパティを返します。 この変更は、スキーマには影響しません。 
  
MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空にすることができます。  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目

- [CompleteNameType](https://msdn.microsoft.com/library/ExchangeWebServices.CompleteNameType.aspx)
- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)
- [連絡先 (Exchange Web サービス) を作成します。](http://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)

