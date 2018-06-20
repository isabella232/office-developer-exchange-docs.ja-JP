---
title: PermissionSet (CalendarPermissionSetType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PermissionSet
api_type:
- schema
ms.assetid: 75f20033-85eb-4627-b4f8-be85e4889e96
description: PermissionSet 要素には、予定表フォルダーに対して構成されているすべてのアクセス許可が含まれています。
ms.openlocfilehash: b2e642fd2ee8ded4d0d4c67509a5587f7b1efa8a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832728"
---
# <a name="permissionset-calendarpermissionsettype"></a>PermissionSet (CalendarPermissionSetType)

**PermissionSet**要素には、予定表フォルダーに対して構成されているすべてのアクセス許可が含まれています。 
  
```XML
<PermissionSet>
   <CalendarPermissions/>
   <UnknownEntries/>
</PermissionSet>
```

 **CalendarPermissonSetType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[CalendarPermissions](calendarpermissions.md) <br/> |フォルダーのアクセス許可を予定表の配列が含まれています。 この要素は、Exchange 2007 SP1 で導入されました。  <br/> |
|[UnknownEntries](unknownentries.md) <br/> |Active Directory ディレクトリ サービスに対して解決できない不明なエントリの配列が含まれています。 この要素は、Exchange 2007 SP1 で導入されました。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[CalendarFolder](calendarfolder.md) <br/> |主に予定表のアイテムを含むフォルダーを表します。  <br/> |
   
## <a name="remarks"></a>備考

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
この要素は、Exchange Server 2007 Service Pack 1 (SP1) で導入されました。
  
### <a name="version-differences"></a>バージョンの相違点

アプリケーションを対象とする Exchange のオンライン、Office 365 の一部として Exchange のオンライン、または、設置型バージョンの Exchange から Exchange 2013 では、フォルダーのアクセス許可は返されません[BaseShape](baseshape.md)の要素に**AllProperties**の値が設定されている場合[GetFolder](getfolder-operation.md)操作要求します。 フォルダーのアクセス許可を取得するには、 **GetFolder**要求内の[AdditionalProperties](additionalproperties.md)要素に[PermissionSet (PermissionSetType)](permissionset-permissionsettype.md)の要素を追加します。 
  
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

