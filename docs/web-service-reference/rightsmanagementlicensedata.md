---
title: RightsManagementLicenseData
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 38f0b7f4-2338-4e90-af67-e0951e8edfa3
description: RightsManagementLicenseData 要素は、アイテムの権限管理のライセンスに関する情報を指定します。
ms.openlocfilehash: ec2ba1dc155afe239c499246095f86fc621910a9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833234"
---
# <a name="rightsmanagementlicensedata"></a><span data-ttu-id="406de-103">RightsManagementLicenseData</span><span class="sxs-lookup"><span data-stu-id="406de-103">RightsManagementLicenseData</span></span>

<span data-ttu-id="406de-104">**RightsManagementLicenseData**要素は、アイテムの権限管理のライセンスに関する情報を指定します。</span><span class="sxs-lookup"><span data-stu-id="406de-104">The **RightsManagementLicenseData** element specifies information about the rights management license for an item.</span></span> 
  
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

 <span data-ttu-id="406de-105">**RightsManagementLicenseDataType**</span><span class="sxs-lookup"><span data-stu-id="406de-105">**RightsManagementLicenseDataType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="406de-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="406de-106">Attributes and elements</span></span>

<span data-ttu-id="406de-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="406de-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="406de-108">属性</span><span class="sxs-lookup"><span data-stu-id="406de-108">Attributes</span></span>

<span data-ttu-id="406de-109">なし。</span><span class="sxs-lookup"><span data-stu-id="406de-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="406de-110">子要素</span><span class="sxs-lookup"><span data-stu-id="406de-110">Child elements</span></span>

<span data-ttu-id="406de-111">[RightsManagedMessageDecryptionStatus](rightsmanagedmessagedecryptionstatus.md) | [RMSTemplateId](rmstemplateid.md) | [TemplateName](templatename.md) | [TemplateDescription](templatedescription.md) | [EditAllowed](editallowed.md) | [ReplyAllowed](replyallowed.md)  |  [ReplyAllAllowed](replyallallowed.md) | [ForwardAllowed](forwardallowed.md) | [ModifyRecipientsAllowed](modifyrecipientsallowed.md) | [ExtractAllowed](extractallowed.md) | [PrintAllowed](printallowed.md) | [ExportAllowed](exportallowed.md)  |  [ProgrammaticAccessAllowed](programmaticaccessallowed.md) | [IsOwner](isowner.md) | [ContentOwner](contentowner.md) | [ContentExpiryDate](contentexpirydate.md)</span><span class="sxs-lookup"><span data-stu-id="406de-111">[RightsManagedMessageDecryptionStatus](rightsmanagedmessagedecryptionstatus.md) | [RMSTemplateId](rmstemplateid.md) | [TemplateName](templatename.md) | [TemplateDescription](templatedescription.md) | [EditAllowed](editallowed.md) | [ReplyAllowed](replyallowed.md) | [ReplyAllAllowed](replyallallowed.md) | [ForwardAllowed](forwardallowed.md) | [ModifyRecipientsAllowed](modifyrecipientsallowed.md) | [ExtractAllowed](extractallowed.md) | [PrintAllowed](printallowed.md) | [ExportAllowed](exportallowed.md) | [ProgrammaticAccessAllowed](programmaticaccessallowed.md) | [IsOwner](isowner.md) | [ContentOwner](contentowner.md) | [ContentExpiryDate](contentexpirydate.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="406de-112">親要素</span><span class="sxs-lookup"><span data-stu-id="406de-112">Parent elements</span></span>

<span data-ttu-id="406de-113">[項目](item.md) | [メッセージ](message-ex15websvcsotherref.md) | [MeetingMessage](meetingmessage.md) | [MeetingRequest](meetingrequest.md) | [MeetingResponse](meetingresponse.md) | [MeetingCancellation](meetingcancellation.md) | [作業](task.md) | [PostItem](postitem.md)  | [カレンダー項目](calendaritem.md) | [連絡先](contact.md) | [DistributionList](distributionlist.md)</span><span class="sxs-lookup"><span data-stu-id="406de-113">[Item](item.md) | [Message](message-ex15websvcsotherref.md) | [MeetingMessage](meetingmessage.md) | [MeetingRequest](meetingrequest.md) | [MeetingResponse](meetingresponse.md) | [MeetingCancellation](meetingcancellation.md) | [Task](task.md) | [PostItem](postitem.md) | [CalendarItem](calendaritem.md) | [Contact](contact.md) | [DistributionList](distributionlist.md)</span></span>
  
## <a name="remarks"></a><span data-ttu-id="406de-114">備考</span><span class="sxs-lookup"><span data-stu-id="406de-114">Remarks</span></span>

<span data-ttu-id="406de-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="406de-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="406de-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="406de-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="406de-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="406de-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="406de-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="406de-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="406de-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="406de-119">Schema name</span></span>  <br/> |<span data-ttu-id="406de-120">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="406de-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="406de-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="406de-121">Validation file</span></span>  <br/> |<span data-ttu-id="406de-122">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="406de-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="406de-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="406de-123">Can be empty</span></span>  <br/> ||
   

