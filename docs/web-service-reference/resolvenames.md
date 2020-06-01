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
description: ResolveNames 要素は、あいまいな名前を解決する要求を定義します。
ms.openlocfilehash: 9c36a5f84451f91e90a8e7148cf384b5cacd7f29
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467950"
---
# <a name="resolvenames"></a>ResolveNames

**ResolveNames**要素は、あいまいな名前を解決する要求を定義します。 
  
```XML
<ResolveNames ReturnFullContactData="" SearchScope="" ContactDataShape="">
   <ParentFolderIds/>
   <UnresolvedEntry/>
</ResolveNames>
```

 **ResolveNamesType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**ReturnFullContactData** <br/> |解決された名前のパブリック連絡先の完全な連絡先の詳細を応答で返すかどうかを指定します。 この属性は、パブリック連絡先に必要です。 この値は、[ [ItemId](itemid.md) ] が常に返されるプライベート連絡先とプライベート配布リストには影響しません。  <br/> |
|**SearchScope** <br/> |ResolveNames 検索の順序と範囲を指定します。  <br/> |
|ContactDataShape  <br/> |連絡先に対して返されるプロパティセットを識別します。 この属性は、Exchange Server 2010 Service Pack 2 (SP2) で導入されました。  <br/> |
   
#### <a name="returnfullcontactdata-attribute-values"></a>ReturnFullContactData 属性値

|**値**|**説明**|
|:-----|:-----|
|True  <br/> |パブリック連絡先の完全な連絡先の詳細が返されます。  <br/> |
|正しくない  <br/> |パブリック連絡先の完全な連絡先の詳細は返されません。  <br/> |
   
#### <a name="searchscope-attribute-values"></a>SearchScope 属性の値

|**値**|**説明**|
|:-----|:-----|
|ActiveDirectory  <br/> |Active Directory ディレクトリサービスのみが検索されます。  <br/> |
|ActiveDirectoryContacts  <br/> |Active Directory が最初に検索され、 [ParentFolderIds](parentfolderids.md)プロパティに指定されている連絡先フォルダーが検索されます。  <br/> |
|連絡先  <br/> |[ParentFolderIds](parentfolderids.md)プロパティによって識別される連絡先フォルダーのみが検索されます。  <br/> |
|ContactsActiveDirectory  <br/> |[ParentFolderIds](parentfolderids.md)プロパティによって識別された連絡先フォルダーが最初に検索されてから、Active Directory が検索されます。  <br/> |
   
#### <a name="contactdatashape-attribute-values"></a>ContactDataShape 属性の値

|**値**|**説明**|
|:-----|:-----|
|IdOnly  <br/> |連絡先アイテムの識別子のプロパティが返されます。  <br/> |
|既定  <br/> |連絡先アイテムのプロパティの既定のセットが返されます。 詳細については、「 [EWS での応答の図形](https://msdn.microsoft.com/library/1c5ddc0a-c4e0-4488-8972-7543b5b464df%28Office.15%29.aspx)」を参照してください。  <br/> |
|AllProperties  <br/> |連絡先アイテムのプロパティの AllProperties セットが返されます。 詳細については、「 [EWS での応答の図形](https://msdn.microsoft.com/library/1c5ddc0a-c4e0-4488-8972-7543b5b464df%28Office.15%29.aspx)」を参照してください。  <br/> |
   
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[ParentFolderIds](parentfolderids.md) <br/> |**Searchscope**属性が ActiveDirectoryContacts、Contacts、または ContactsActiveDirectory に設定されている場合に検索される連絡先フォルダーの識別子の配列を格納します。 ParentFolderIds 配列には、1つの連絡先フォルダーの識別子のみを含めることができます。 **ParentFolderIds**要素が存在しない場合は、既定の連絡先フォルダーが検索されます。  <br/> 代理人アクセスには、フォルダー識別子を使用できます。  <br/> Active Directory 検索は、アクセス制御リスト (Acl) を使用して実行されます。 一部のユーザーは、一部の Active Directory オブジェクトを表示する権限を持っていない場合があります。  <br/> この要素は省略できます。  <br/> |
|[UnresolvedEntry](unresolvedentry.md) <br/> |解決する連絡先または配布リストの名前を格納します。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空にすることができます。  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



[ResolveNames 操作](resolvenames-operation.md)
  
[ResolveNamesType](https://msdn.microsoft.com/library/ExchangeWebServices.ResolveNamesType.aspx)
  
[ResolveNamesSearchScopeType](https://msdn.microsoft.com/library/ExchangeWebServices.ResolveNamesSearchScopeType.aspx)


- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)


[名前解決の使用](https://msdn.microsoft.com/library/9257fb07-89d2-46eb-b885-e2173fe6fbc1%28Office.15%29.aspx)

