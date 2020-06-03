---
title: ExpandGroupMembership
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 8989e96b-8fa1-4858-93b2-2cbdb30b9ca9
description: ExpandGroupMembership 要素は、Getsearchablemailemailrequest 要求から返されるグループのメンバーシップを拡張するかどうかを示します。
ms.openlocfilehash: 8a94aa3da165ecc13282127e75c8d166f3972ead
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456907"
---
# <a name="expandgroupmembership"></a>ExpandGroupMembership

**Expandgroupmembership**要素は、 **Getsearchablemailemailrequest**要求から返されるグループのメンバーシップを拡張するかどうかを示します。 
  
```XML
<ExpandGroupMembership>true | false</ExpandGroupMembership>
```

 **Boolean**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[Getdiscoverysearchconfiguration](getdiscoverysearchconfiguration.md)  | [Getsearchablemailemailボックス](getsearchablemailboxes.md)
  
## <a name="text-value"></a>テキスト値

**Expandgroupelement**要素のテキスト値が**true**である場合、グループメンバーシップが展開されていることを示します。 値が**false**の場合は、グループのメンバーシップが展開されていないことを示します。グループのメンバーが表示されます。 
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空にすることができます。  <br/> |false  <br/> |
   

