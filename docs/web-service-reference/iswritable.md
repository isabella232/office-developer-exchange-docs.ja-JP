---
title: IsWritable 可能
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: d4af8eee-7001-4a8e-b9bd-d14882f2406b
description: IsWritable 可能要素は、基になる連絡先または Active Directory 受信者に書き込むことができるかどうかを指定します。
ms.openlocfilehash: 96075adc1772027456f8829eee43bdc734644c09
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467572"
---
# <a name="iswritable"></a>IsWritable 可能

**Iswritable 可能**要素は、基になる連絡先または Active Directory 受信者に書き込むことができるかどうかを指定します。 
  
```XML
<IsWritable> true | false </IsWritable>
```

 **Boolean**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[属性 (PersonaAttributionType)](attribution-personaattributiontype.md)
  
## <a name="text-value"></a>テキスト値

**Iswritable**要素のテキスト値が**true**の場合は、連絡先または Active Directory オブジェクトが書き込みアクセスで利用可能であることを示します。 値が**false**の場合は、連絡先または Active Directory オブジェクトが書き込みアクセスで利用できないことを示します。 
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  

