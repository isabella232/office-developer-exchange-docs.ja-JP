---
title: RightsManagementLicenseData
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 38f0b7f4-2338-4e90-af67-e0951e8edfa3
description: RightsManagementLicenseData 要素は、アイテムの権限管理ライセンスに関する情報を指定します。
ms.openlocfilehash: 8875e9bad425224f86b6de5149f87a36c2a2581e
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59523469"
---
# <a name="rightsmanagementlicensedata"></a>RightsManagementLicenseData

**RightsManagementLicenseData** 要素は、アイテムの権限管理ライセンスに関する情報を指定します。 
  
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

[RightsManagedMessageDecryptionStatus](rightsmanagedmessagedecryptionstatus.md)  | [RMSTemplateId](rmstemplateid.md)  | [TemplateName](templatename.md)  | [TemplateDescription](templatedescription.md)  | [EditAllowed](editallowed.md)  | [ReplyAllowed](replyallowed.md)  | [ReplyAllAllowed](replyallallowed.md)  | [ForwardAllowed](forwardallowed.md)  | [ModifyRecipientsAllowed](modifyrecipientsallowed.md)  | [ExtractAllowed](extractallowed.md)  | [PrintAllowed](printallowed.md)  | [ExportAllowed](exportallowed.md)  | [ProgrammaticAccessAllowed](programmaticaccessallowed.md)  | [IsOwner](isowner.md)  | [ContentOwner](contentowner.md)  | [ContentExpiryDate](contentexpirydate.md)
  
### <a name="parent-elements"></a>親要素

[アイテム](item.md)  | [メッセージ](message-ex15websvcsotherref.md)  | [MeetingMessage](meetingmessage.md)  | [MeetingRequest](meetingrequest.md)  | [MeetingResponse](meetingresponse.md)  | [MeetingCancellation](meetingcancellation.md)  | [タスク](task.md)  | [PostItem](postitem.md)  | [CalendarItem](calendaritem.md)  | [連絡先](contact.md)  | [DistributionList](distributionlist.md)
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空の場合  <br/> ||
   

