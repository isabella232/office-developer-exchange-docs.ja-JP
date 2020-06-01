---
title: RightsManagementLicenseData
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 38f0b7f4-2338-4e90-af67-e0951e8edfa3
description: RightsManagementLicenseData 要素は、アイテムの権限管理ライセンスに関する情報を指定します。
ms.openlocfilehash: 892edfd6775838b1e6329e8db0ee9bb8e3c519ff
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463189"
---
# <a name="rightsmanagementlicensedata"></a>RightsManagementLicenseData

**RightsManagementLicenseData**要素は、アイテムの権限管理ライセンスに関する情報を指定します。 
  
```XML
<RightsManagementLicenseData>
   <RightsManagedMessageDecryptionStatus/>
   <RmsTemplateId/>
   <TemplateName/>
   <TemplateDescription/>
   <EditAllowed/>
   <ReplyAllowed/>
   <ReplyAllAllowed/>
   <ForwardAllowed/>
   <ModifyRecipientsAllowed/>
   <ExtractAllowed/>
   <PrintAllowed/>
   <ExportAllowed/>
   <ProgrammaticAccessAllowed/>
   <IsOwner/>
   <ContentOwner/>
   <ContentExpiryDate/>
</RightsManagementLicenseData>
```

 **RightsManagementLicenseDataType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

[RightsManagedMessageDecryptionStatus](rightsmanagedmessagedecryptionstatus.md)  | [RMSTemplateId](rmstemplateid.md)  | [TemplateName](templatename.md)  | [Templatedescription](templatedescription.md)  | [Editallowed](editallowed.md)  | [ReplyAllowed](replyallowed.md)  | [ReplyAllAllowed](replyallallowed.md)  | [Forwardallowed](forwardallowed.md)  | [Modify受信者の許可](modifyrecipientsallowed.md)  | [ExtractAllowed](extractallowed.md)  | [Printallowed](printallowed.md)  | [Exportallowed](exportallowed.md)  | [ProgrammaticAccessAllowed](programmaticaccessallowed.md)  | [Isowner](isowner.md)  |  場合[ContentOwner](contentowner.md)  | [ContentExpiryDate](contentexpirydate.md)
  
### <a name="parent-elements"></a>親要素

[アイテム](item.md)  | [メッセージ](message-ex15websvcsotherref.md)  | [会議メッセージ](meetingmessage.md)  | [会議の要求](meetingrequest.md)  | [会議の応答](meetingresponse.md)  | [会議のキャンセル](meetingcancellation.md)  | [タスク](task.md)  | [Postitem](postitem.md)  | [Calendaritem](calendaritem.md)  | [連絡先](contact.md)  | [DistributionList](distributionlist.md)
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空にすることができます。  <br/> ||
   

