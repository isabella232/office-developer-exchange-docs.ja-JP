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
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463189"
---
# <a name="rightsmanagementlicensedata"></a><span data-ttu-id="23e47-103">RightsManagementLicenseData</span><span class="sxs-lookup"><span data-stu-id="23e47-103">RightsManagementLicenseData</span></span>

<span data-ttu-id="23e47-104">**RightsManagementLicenseData**要素は、アイテムの権限管理ライセンスに関する情報を指定します。</span><span class="sxs-lookup"><span data-stu-id="23e47-104">The **RightsManagementLicenseData** element specifies information about the rights management license for an item.</span></span> 
  
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

 <span data-ttu-id="23e47-105">**RightsManagementLicenseDataType**</span><span class="sxs-lookup"><span data-stu-id="23e47-105">**RightsManagementLicenseDataType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="23e47-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="23e47-106">Attributes and elements</span></span>

<span data-ttu-id="23e47-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="23e47-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="23e47-108">属性</span><span class="sxs-lookup"><span data-stu-id="23e47-108">Attributes</span></span>

<span data-ttu-id="23e47-109">なし。</span><span class="sxs-lookup"><span data-stu-id="23e47-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="23e47-110">子要素</span><span class="sxs-lookup"><span data-stu-id="23e47-110">Child elements</span></span>

<span data-ttu-id="23e47-111">[RightsManagedMessageDecryptionStatus](rightsmanagedmessagedecryptionstatus.md)  | [RMSTemplateId](rmstemplateid.md)  | [TemplateName](templatename.md)  | [Templatedescription](templatedescription.md)  | [Editallowed](editallowed.md)  | [ReplyAllowed](replyallowed.md)  | [ReplyAllAllowed](replyallallowed.md)  | [Forwardallowed](forwardallowed.md)  | [Modify受信者の許可](modifyrecipientsallowed.md)  | [ExtractAllowed](extractallowed.md)  | [Printallowed](printallowed.md)  | [Exportallowed](exportallowed.md)  | [ProgrammaticAccessAllowed](programmaticaccessallowed.md)  | [Isowner](isowner.md)  |  場合[ContentOwner](contentowner.md)  | [ContentExpiryDate](contentexpirydate.md)</span><span class="sxs-lookup"><span data-stu-id="23e47-111">[RightsManagedMessageDecryptionStatus](rightsmanagedmessagedecryptionstatus.md) | [RMSTemplateId](rmstemplateid.md) | [TemplateName](templatename.md) | [TemplateDescription](templatedescription.md) | [EditAllowed](editallowed.md) | [ReplyAllowed](replyallowed.md) | [ReplyAllAllowed](replyallallowed.md) | [ForwardAllowed](forwardallowed.md) | [ModifyRecipientsAllowed](modifyrecipientsallowed.md) | [ExtractAllowed](extractallowed.md) | [PrintAllowed](printallowed.md) | [ExportAllowed](exportallowed.md) | [ProgrammaticAccessAllowed](programmaticaccessallowed.md) | [IsOwner](isowner.md) | [ContentOwner](contentowner.md) | [ContentExpiryDate](contentexpirydate.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="23e47-112">親要素</span><span class="sxs-lookup"><span data-stu-id="23e47-112">Parent elements</span></span>

<span data-ttu-id="23e47-113">[アイテム](item.md)  | [メッセージ](message-ex15websvcsotherref.md)  | [会議メッセージ](meetingmessage.md)  | [会議の要求](meetingrequest.md)  | [会議の応答](meetingresponse.md)  | [会議のキャンセル](meetingcancellation.md)  | [タスク](task.md)  | [Postitem](postitem.md)  | [Calendaritem](calendaritem.md)  | [連絡先](contact.md)  | [DistributionList](distributionlist.md)</span><span class="sxs-lookup"><span data-stu-id="23e47-113">[Item](item.md) | [Message](message-ex15websvcsotherref.md) | [MeetingMessage](meetingmessage.md) | [MeetingRequest](meetingrequest.md) | [MeetingResponse](meetingresponse.md) | [MeetingCancellation](meetingcancellation.md) | [Task](task.md) | [PostItem](postitem.md) | [CalendarItem](calendaritem.md) | [Contact](contact.md) | [DistributionList](distributionlist.md)</span></span>
  
## <a name="remarks"></a><span data-ttu-id="23e47-114">注釈</span><span class="sxs-lookup"><span data-stu-id="23e47-114">Remarks</span></span>

<span data-ttu-id="23e47-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="23e47-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="23e47-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="23e47-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="23e47-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="23e47-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="23e47-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="23e47-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="23e47-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="23e47-119">Schema name</span></span>  <br/> |<span data-ttu-id="23e47-120">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="23e47-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="23e47-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="23e47-121">Validation file</span></span>  <br/> |<span data-ttu-id="23e47-122">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="23e47-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="23e47-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="23e47-123">Can be empty</span></span>  <br/> ||
   

