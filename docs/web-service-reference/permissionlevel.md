---
title: PermissionLevel
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- PermissionLevel
api_type:
- schema
ms.assetid: 87978600-3523-451e-a725-ef092c543e2a
description: PermissionLevel 要素は、ユーザーがフォルダーに持つアクセス許可レベルを表します。 この要素は、2007 Microsoft Exchange Server パック 1 (SP1) で導入されました。
ms.openlocfilehash: 48b8db48afe6ced137acceeade2911a044298d75
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59544837"
---
# <a name="permissionlevel"></a>PermissionLevel

**PermissionLevel 要素** は、ユーザーがフォルダーに持つアクセス許可レベルを表します。 この要素は、2007 Microsoft Exchange Server パック 1 (SP1) で導入されました。 
  
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
|[アクセス許可](permission.md) <br/> |ユーザーがフォルダーに対して持つアクセスを定義します。 この要素は、2007 SP1 Exchange導入されました。  <br/> |
   
## <a name="text-value"></a>テキスト値

次の表に、PermissionLevel 要素に使用できる **値を示** します。 
  
**PermissionLevel 要素のテキスト値**

|**値**|**説明**|
|:-----|:-----|
|なし  <br/> |ユーザーがフォルダーに対するアクセス許可を持たなかどうかを示します。  <br/> |
|Owner  <br/> |ユーザーがフォルダー内のすべてのアイテムを作成、読み取り、編集、および削除し、サブフォルダーを作成できます。 ユーザーは、フォルダー所有者とフォルダー連絡先の両方です。  <br/> |
|PublishingEditor (出版編集者)  <br/> |ユーザーがフォルダー内のすべてのアイテムを作成、読み取り、編集、および削除し、サブフォルダーを作成できます。  <br/> |
|エディター  <br/> |ユーザーがフォルダー内のすべてのアイテムを作成、読み取り、編集、および削除できる状態を示します。  <br/> |
|PublishingAuthor (出版著者)  <br/> |ユーザーがフォルダー内のすべてのアイテムを作成および読み取り、ユーザーが作成したアイテムのみを編集および削除し、サブフォルダーを作成できます。  <br/> |
|Author  <br/> |ユーザーがフォルダー内のすべてのアイテムを作成および読み取り、ユーザーが作成したアイテムのみを編集および削除できます。  <br/> |
|NoneditingAuthor (非編集著者)  <br/> |ユーザーがフォルダー内のすべてのアイテムを作成および読み取り、ユーザーが作成したアイテムのみを削除できます。  <br/> |
|レビュー担当者  <br/> |ユーザーがフォルダー内のすべてのアイテムを読み取り可能な状態を示します。  <br/> |
|共同作成者  <br/> |ユーザーがフォルダー内にアイテムを作成できる状態を示します。 フォルダーの内容は表示されません。  <br/> |
|Custom  <br/> |ユーザーがフォルダーに対するカスタム アクセス許可を持っているかどうかを示します。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)


[アクセス許可Folder-Level設定する](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

