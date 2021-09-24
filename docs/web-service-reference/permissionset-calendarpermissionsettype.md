---
title: PermissionSet (CalendarPermissionSetType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- PermissionSet
api_type:
- schema
ms.assetid: 75f20033-85eb-4627-b4f8-be85e4889e96
description: PermissionSet 要素には、予定表フォルダー用に構成されているすべてのアクセス許可が含まれる。
ms.openlocfilehash: 26351be8fd9fbe56ea5abb2dd346cb9c9458c463
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59539155"
---
# <a name="permissionset-calendarpermissionsettype"></a>PermissionSet (CalendarPermissionSetType)

**PermissionSet 要素** には、予定表フォルダー用に構成されているすべてのアクセス許可が含まれる。 
  
```XML
<PermissionSet>
   <CalendarPermissions/>
   <UnknownEntries/>
</PermissionSet>
```

 **CalendarPermissonSetType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[CalendarPermissions](calendarpermissions.md) <br/> |フォルダーの予定表のアクセス許可の配列を含む。 この要素は、2007 SP1 Exchange導入されました。  <br/> |
|[UnknownEntries](unknownentries.md) <br/> |Active Directory ディレクトリ サービスに対して解決できない不明なエントリの配列が含まれます。 この要素は、2007 SP1 Exchange導入されました。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[CalendarFolder](calendarfolder.md) <br/> |主に予定表アイテムを含むフォルダーを表します。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
この要素は、Exchange Server 2007 Service Pack 1 (SP1) で導入されました。
  
### <a name="version-differences"></a>バージョンの相違点

Office 365 の一部として Exchange Online、Exchange Online、または Exchange 2013 から始まるオンプレミスバージョンの Exchange を対象とするアプリケーションの場合 [、BaseShape](baseshape.md)要素に [GetFolder](getfolder-operation.md)の **AllProperties** の値がある場合、フォルダーのアクセス許可は返されません。操作要求。 フォルダーのアクセス許可を取得するには、GetFolder 要求の [AdditionalProperties](additionalproperties.md)要素に [PermissionSet (PermissionSetType)](permissionset-permissionsettype.md)要素 **を追加** します。 
  
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

