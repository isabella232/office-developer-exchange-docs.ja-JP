---
title: Entry (PhoneNumber)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Entry
api_type:
- schema
ms.assetid: e3d0a4d5-8af8-4607-aa2e-ef3111b63b55
description: Entry 要素は、連絡先の電話番号を表します。
ms.openlocfilehash: 62f7091bb750dc7ca74b1e5637a437e2cdad4f1c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459638"
---
# <a name="entry-phonenumber"></a>Entry (PhoneNumber)

**Entry**要素は、連絡先の電話番号を表します。 
  
```xml
<Entry Key=""/>
```

 **PhoneNumberDictionaryEntryType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**Key** <br/> | 電話番号を識別します。 キー属性の型は**PhoneNumberKeyType**です。<br/><br/> 次に、この属性で使用できる値を示します。<br/><br/>- AssistantPhone  <br/>-BusinessFax  <br/>- BusinessPhone  <br/>- BusinessPhone2  <br/>-コールバック  <br/>-CarPhone  <br/>-会社の Mainphone  <br/>-ホーム Fax  <br/>-HomePhone  <br/>- HomePhone2  <br/>-Isdn  <br/>-MobilePhone  <br/>-他の Fax  <br/>-他の電話  <br/>-ポケットベル  <br/>- PrimaryPhone  <br/>- RadioPhone  <br/>-テレックス  <br/>-TtyTddPhone  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[PhoneNumbers](phonenumbers.md) <br/> |連絡先の電話番号のコレクションを表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

この要素を使用する場合は、電話番号を表すテキスト値が必要です。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空にすることができます。  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目

- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)
- [連絡先の作成 (Exchange Web サービス)](https://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx) 
- [連絡先の更新](https://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx)  
- [連絡先の削除](https://msdn.microsoft.com/library/fcc3dc84-cd3e-455e-a1a7-ae6921c9b588%28Office.15%29.aspx)

