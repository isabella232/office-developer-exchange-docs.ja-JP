---
title: CalendarPermissionLevel
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CalendarPermissionLevel
api_type:
- schema
ms.assetid: 6ac2b792-4326-4a3f-b6cb-977bf523b5b2
description: CalendarPermissionLevel 要素は、ユーザーが予定表フォルダーに対して持っているアクセス許可レベルを表します。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。
ms.openlocfilehash: 670f78e0b3cef7a40339c83d84916871f8969536
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527181"
---
# <a name="calendarpermissionlevel"></a>CalendarPermissionLevel

**Calendarpermissionlevel**要素は、ユーザーが予定表フォルダーに対して持っているアクセス許可レベルを表します。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。 
  
```xml
<CalendarPermissionLevel>None or Owner or PublishingEditor or Editor or PublishingAuthor or Author or NoneditingAuthor or Reviewer or Contributor or FreeBusyTimeOnly or FreeBusyTimeAndSubjectAndLocation or Custom</CalendarPermissionLevel>
```

 **CalendarPermissionLevelType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[CalendarPermission](calendarpermission.md) <br/> |ユーザーが予定表フォルダーに対して持っているアクセス権を定義します。 この要素は、Exchange 2007 SP1 で導入されました。  <br/> |
   
## <a name="text-value"></a>テキスト値

次の表に、 **Calendarpermissionlevel**要素に指定できる値を示します。 
  
**CalendarPermissionLevel 要素のテキスト値**

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
|FreeBusyTimeOnly  <br/> |ユーザーが予定表内でのみ空き時間情報を表示できることを示します。  <br/> |
|FreeBusyTimeAndSubjectAndLocation  <br/> |ユーザーが予定表内の空き時間情報を表示できること、および予定の件名と場所を表示できることを示します。  <br/> |
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

