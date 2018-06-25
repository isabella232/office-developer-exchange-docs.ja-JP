---
title: ResolveNames
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ResolveNames
api_type:
- schema
ms.assetid: c85207e1-1315-443b-94ec-2b58f405076b
description: ResolveNames 要素では、あいまいな名前を解決する要求を定義します。
ms.openlocfilehash: e97b6e78d99cf8ffa3d680907916882d40963f59
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833172"
---
# <a name="resolvenames"></a>ResolveNames

**ResolveNames**要素では、あいまいな名前を解決する要求を定義します。 
  
```XML
<ResolveNames ReturnFullContactData="" SearchScope="" ContactDataShape="">
   <ParentFolderIds/>
   <UnresolvedEntry/>
</ResolveNames>
```

 **ResolveNamesType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**ReturnFullContactData** <br/> |解決された名前の公開アドレス帳の完全な連絡先の詳細が応答で返されるかどうかについて説明します。 この属性は、パブリック メンバーに必要です。 この値は、プライベートの連絡先と個人用配布リスト、[アイテム Id](itemid.md)が常に返されるには影響しません。  <br/> |
|**SearchScope** <br/> |ResolveNames 検索範囲の順序を識別します。  <br/> |
|ContactDataShape  <br/> |連絡先に対して返されるプロパティを識別します。 この属性は、Exchange Server 2010 のサービス パック 2 (SP2) で導入されました。  <br/> |
   
#### <a name="returnfullcontactdata-attribute-values"></a>ReturnFullContactData 属性の値

|**値**|**説明**|
|:-----|:-----|
|True  <br/> |公開アドレス帳の完全な連絡先の詳細情報が返されます。  <br/> |
|False  <br/> |公開アドレス帳の完全な連絡先の詳細情報は返されません。  <br/> |
   
#### <a name="searchscope-attribute-values"></a>SearchScope 属性の値

|**値**|**説明**|
|:-----|:-----|
|ActiveDirectory  <br/> |Active Directory ディレクトリ サービスのみが検索されます。  <br/> |
|ActiveDirectoryContacts  <br/> |最初に active Directory を検索し、 [ParentFolderIds](parentfolderids.md)プロパティで指定されている連絡先フォルダーを検索し、します。  <br/> |
|連絡先  <br/> |[ParentFolderIds](parentfolderids.md)プロパティによって指定されている連絡先フォルダーのみが検索されます。  <br/> |
|ContactsActiveDirectory  <br/> |[ParentFolderIds](parentfolderids.md)プロパティによって指定されている連絡先フォルダーを最初に検索され、Active Directory を検索します。  <br/> |
   
#### <a name="contactdatashape-attribute-values"></a>ContactDataShape 属性の値

|**値**|**説明**|
|:-----|:-----|
|IdOnly  <br/> |連絡先アイテムの id プロパティが返されます。  <br/> |
|Default  <br/> |連絡先アイテムのプロパティの既定のセットが返されます。 詳細については、 [EWS の避難用図形](http://msdn.microsoft.com/library/1c5ddc0a-c4e0-4488-8972-7543b5b464df%28Office.15%29.aspx)を参照してください。  <br/> |
|AllProperties  <br/> |連絡先アイテムのプロパティの AllProperties のセットが返されます。 詳細については、 [EWS の避難用図形](http://msdn.microsoft.com/library/1c5ddc0a-c4e0-4488-8972-7543b5b464df%28Office.15%29.aspx)を参照してください。  <br/> |
   
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[ParentFolderIds](parentfolderids.md) <br/> |**SearchScope**属性は、ActiveDirectoryContacts、連絡先、または ContactsActiveDirectory に設定されている場合を検索する連絡先フォルダー識別子の配列が含まれています。 ParentFolderIds アレイでは、1 つの連絡先フォルダーの識別子を含めることができますのみです。 **ParentFolderIds**要素が存在しない場合は、既定の連絡先フォルダーが検索されます。  <br/> フォルダーの識別子は、代理人アクセスを使用できます。  <br/> 作業中のディレクトリ検索は、アクセス制御リスト (Acl) を使用して実行されます。 一部のユーザーは、いくつかの Active Directory オブジェクトを表示する権限をいない可能性があります。  <br/> この要素はオプションです。  <br/> |
|[UnresolvedEntry](unresolvedentry.md) <br/> |解決するのには、連絡先または配布リストの名前が含まれています。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="remarks"></a>備考

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空にすることができます。  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



[ResolveNames 操作](resolvenames-operation.md)
  
[ResolveNamesType](https://msdn.microsoft.com/library/ExchangeWebServices.ResolveNamesType.aspx)
  
[ResolveNamesSearchScopeType](https://msdn.microsoft.com/library/ExchangeWebServices.ResolveNamesSearchScopeType.aspx)


- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)


[名前解決の使用](http://msdn.microsoft.com/library/9257fb07-89d2-46eb-b885-e2173fe6fbc1%28Office.15%29.aspx)

