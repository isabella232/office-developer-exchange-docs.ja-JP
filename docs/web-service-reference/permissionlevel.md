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
description: PermissionLevel 要素は、ユーザーがフォルダーに必要なアクセス許可レベルを表します。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。
ms.openlocfilehash: 7cc734f5807fe039467065315c220341f47d3fb4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832730"
---
# <a name="permissionlevel"></a>PermissionLevel

**PermissionLevel**要素は、ユーザーがフォルダーに必要なアクセス許可レベルを表します。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。 
  
```xml
<PermissionLevel>None or Owner or PublishingEditor or Editor or PublishingAuthor or Author or NoneditingAuthor or Reviewer or Contributor or Custom</PermissionLevel>
```

 **PermissionLevelType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[Permission](permission.md) <br/> |フォルダーにユーザーが持つアクセス権を定義します。 この要素は、Exchange 2007 SP1 で導入されました。  <br/> |
   
## <a name="text-value"></a>テキスト値

次の表は、 **PermissionLevel**要素の値を一覧します。 
  
**PermissionLevel 要素のテキスト値**

|**値**|**説明**|
|:-----|:-----|
|なし  <br/> |そのユーザーの権限を持ってフォルダーを示します。  <br/> |
|Owner  <br/> |ユーザーことができます作成、読み取り、編集、および、フォルダー内のすべてのアイテムを削除およびサブフォルダーを作成することを示します。 ユーザーは、フォルダーの所有者とフォルダーの連絡先の両方です。  <br/> |
|PublishingEditor (出版編集者)  <br/> |ユーザーことができます作成、読み取り、編集、および、フォルダー内のすべてのアイテムを削除およびサブフォルダーを作成することを示します。  <br/> |
|Editor  <br/> |ユーザーが作成、読み取り、編集、およびフォルダー内のすべてのアイテムを削除することを示します。  <br/> |
|PublishingAuthor (出版著者)  <br/> |ユーザーを作成し、フォルダー内のすべてのアイテム編集しユーザーを作成するアイテムのみを削除し、ことサブフォルダーを作成することを示します。  <br/> |
|作成者  <br/> |ユーザーを作成し、フォルダー内のすべてのアイテムし編集および削除できますユーザーが作成したアイテムのみを示します。  <br/> |
|NoneditingAuthor (非編集著者)  <br/> |ユーザーを作成し、フォルダー内のすべてのアイテムを読み取るし、ことユーザーが作成したアイテムのみを削除することを示します。  <br/> |
|Reviewer  <br/> |ユーザーがフォルダー内のすべてのアイテムを読み取ることができますを示します。  <br/> |
|Contributor  <br/> |ユーザーがフォルダーにアイテムを作成できることを示します。 フォルダーの内容は表示されません。  <br/> |
|カスタム  <br/> |ユーザーがフォルダーのカスタム アクセス許可を持っていることを示します。  <br/> |
   
## <a name="remarks"></a>備考

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)


[フォルダー レベルのアクセス許可の設定](http://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

