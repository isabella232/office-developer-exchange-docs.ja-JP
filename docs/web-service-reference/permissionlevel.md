---
title: PermissionLevel
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PermissionLevel
api_type:
- schema
ms.assetid: 87978600-3523-451e-a725-ef092c543e2a
description: PermissionLevel 要素は、ユーザーがフォルダーに対して持っているアクセス許可レベルを表します。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。
ms.openlocfilehash: e1e441c53b5c40c16051eb852a6b35a8af7476e2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458041"
---
# <a name="permissionlevel"></a>PermissionLevel

**Permissionlevel**要素は、ユーザーがフォルダーに対して持っているアクセス許可レベルを表します。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。 
  
```xml
<PermissionLevel>None or Owner or PublishingEditor or Editor or PublishingAuthor or Author or NoneditingAuthor or Reviewer or Contributor or Custom</PermissionLevel>
```

 **PermissionLevelType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[アクセス許可](permission.md) <br/> |ユーザーがフォルダーに対して持つアクセス許可を定義します。 この要素は、Exchange 2007 SP1 で導入されました。  <br/> |
   
## <a name="text-value"></a>テキスト値

次の表に、 **Permissionlevel**要素に指定できる値を示します。 
  
**PermissionLevel 要素のテキスト値**

|**値**|**説明**|
|:-----|:-----|
|なし  <br/> |ユーザーがフォルダーに対するアクセス許可を持っていないことを示します。  <br/> |
|Owner  <br/> |ユーザーがフォルダー内のすべてのアイテムを作成、読み取り、編集、および削除できること、およびサブフォルダーを作成できることを示します。 ユーザーはフォルダーの所有者とフォルダーの両方の連絡先です。  <br/> |
|PublishingEditor (出版編集者)  <br/> |ユーザーがフォルダー内のすべてのアイテムを作成、読み取り、編集、および削除できること、およびサブフォルダーを作成できることを示します。  <br/> |
|エディター  <br/> |ユーザーがフォルダー内のすべてのアイテムを作成、読み取り、編集、および削除できることを示します。  <br/> |
|PublishingAuthor (出版著者)  <br/> |ユーザーがフォルダー内のすべてのアイテムを作成および読み取り、ユーザーが作成したアイテムのみを編集および削除し、サブフォルダーを作成できることを示します。  <br/> |
|設定元  <br/> |ユーザーがフォルダー内のすべてのアイテムを作成および読み取ることができ、ユーザーが作成したアイテムのみを編集および削除できることを示します。  <br/> |
|NoneditingAuthor (非編集著者)  <br/> |ユーザーがフォルダー内のすべてのアイテムを作成および読み取ることができ、ユーザーが作成したアイテムのみを削除できることを示します。  <br/> |
|レビュー担当者  <br/> |ユーザーがフォルダー内のすべてのアイテムを読み取ることができることを示します。  <br/> |
|共同作成者  <br/> |ユーザーがフォルダー内にアイテムを作成できることを示します。 フォルダーの内容は表示されません。  <br/> |
|Custom  <br/> |ユーザーがフォルダーに対して独自のアクセス許可を持っていることを示します。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)


[フォルダーレベルのアクセス許可を設定する](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

