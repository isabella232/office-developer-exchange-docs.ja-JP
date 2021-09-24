---
title: ResolveNames
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ResolveNames
api_type:
- schema
ms.assetid: c85207e1-1315-443b-94ec-2b58f405076b
description: ResolveNames 要素は、あいまいな名前を解決するための要求を定義します。
ms.openlocfilehash: 8fbf933593b43de656bf8731aa86cc8c8eb76bb4
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59514145"
---
# <a name="resolvenames"></a>ResolveNames

**ResolveNames 要素** は、あいまいな名前を解決するための要求を定義します。 
  
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
|**ReturnFullContactData** <br/> |解決された名前のパブリック連絡先の完全な連絡先の詳細が応答で返されるかどうかを示します。 この属性は、パブリック連絡先に必要です。 この値は [、ItemId](itemid.md) が常に返されるプライベート連絡先とプライベート配布リストには影響を与えかねない。  <br/> |
|**SearchScope** <br/> |ResolveNames 検索の順序と範囲を識別します。  <br/> |
|ContactDataShape  <br/> |連絡先に返されるプロパティ セットを識別します。 この属性は、2010 Exchange Server Service Pack 2 (SP2) で導入されました。  <br/> |
   
#### <a name="returnfullcontactdata-attribute-values"></a>ReturnFullContactData 属性値

|**値**|**説明**|
|:-----|:-----|
|True  <br/> |パブリック連絡先の完全な連絡先の詳細が返されます。  <br/> |
|いいえ  <br/> |パブリック連絡先の完全な連絡先の詳細は返されません。  <br/> |
   
#### <a name="searchscope-attribute-values"></a>SearchScope 属性値

|**値**|**説明**|
|:-----|:-----|
|ActiveDirectory  <br/> |Active Directory ディレクトリ サービスだけが検索されます。  <br/> |
|ActiveDirectoryContacts  <br/> |Active Directory が最初に検索され、次に [ParentFolderIds](parentfolderids.md) プロパティで指定された連絡先フォルダーが検索されます。  <br/> |
|連絡先  <br/> |[ParentFolderIds](parentfolderids.md)プロパティによって識別される連絡先フォルダーだけが検索されます。  <br/> |
|ContactsActiveDirectory  <br/> |[ParentFolderIds](parentfolderids.md)プロパティで識別される連絡先フォルダーが最初に検索され、次に Active Directory が検索されます。  <br/> |
   
#### <a name="contactdatashape-attribute-values"></a>ContactDataShape 属性値

|**値**|**説明**|
|:-----|:-----|
|IdOnly  <br/> |連絡先アイテム識別子プロパティが返されます。  <br/> |
|既定値  <br/> |連絡先アイテムのプロパティの既定のセットが返されます。 詳細については [、「EWS の応答図形」を参照してください](https://msdn.microsoft.com/library/1c5ddc0a-c4e0-4488-8972-7543b5b464df%28Office.15%29.aspx)。  <br/> |
|AllProperties  <br/> |連絡先アイテムのプロパティの AllProperties セットが返されます。 詳細については [、「EWS の応答図形」を参照してください](https://msdn.microsoft.com/library/1c5ddc0a-c4e0-4488-8972-7543b5b464df%28Office.15%29.aspx)。  <br/> |
   
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[ParentFolderIds](parentfolderids.md) <br/> |**SearchScope** 属性が ActiveDirectoryContacts、Contact、または ContactsActiveDirectory に設定されている場合に検索される連絡先フォルダー識別子の配列を含みます。 ParentFolderIds 配列には、1 つの連絡先フォルダー識別子のみを含めできます。 **ParentFolderIds** 要素が存在しない場合、既定の連絡先フォルダーが検索されます。  <br/> フォルダー識別子は、代理人アクセスに使用できます。  <br/> Active Directory の検索は、アクセス制御リスト (ACL) を使用して実行されます。 一部のユーザーは、一部の Active Directory オブジェクトを表示する権限を持てない場合があります。  <br/> この要素は省略できます。  <br/> |
|[UnresolvedEntry](unresolvedentry.md) <br/> |解決する連絡先または配布リストの名前が含まれる。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空の場合  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



[ResolveNames 操作](resolvenames-operation.md)
  
[ResolveNamesType](https://msdn.microsoft.com/library/ExchangeWebServices.ResolveNamesType.aspx)
  
[ResolveNamesSearchScopeType](https://msdn.microsoft.com/library/ExchangeWebServices.ResolveNamesSearchScopeType.aspx)


- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)


[名前解決の使用](https://msdn.microsoft.com/library/9257fb07-89d2-46eb-b885-e2173fe6fbc1%28Office.15%29.aspx)

