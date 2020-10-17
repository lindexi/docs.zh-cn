---
ms.openlocfilehash: 584014572ab799e1e3ab2f02c9fbf4fe6b0c17e7
ms.sourcegitcommit: 636af37170ae75a11c4f7d1ecd770820e7dfe7bd
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/07/2020
ms.locfileid: "91804916"
---
### <a name="blazor-updated-browser-support"></a><span data-ttu-id="b2b2d-101">Blazor：更新的浏览器支持</span><span class="sxs-lookup"><span data-stu-id="b2b2d-101">Blazor: Updated browser support</span></span>

<span data-ttu-id="b2b2d-102">ASP.NET Core 5.0 引入了[新的 Blazor 功能](https://github.com/dotnet/aspnetcore/issues/21514)，其中一些功能与旧版浏览器不兼容。</span><span class="sxs-lookup"><span data-stu-id="b2b2d-102">ASP.NET Core 5.0 introduces [new Blazor features](https://github.com/dotnet/aspnetcore/issues/21514), some of which are incompatible with older browsers.</span></span> <span data-ttu-id="b2b2d-103">ASP.NET Core 5.0 中的 Blazor 支持的浏览器列表已相应更新。</span><span class="sxs-lookup"><span data-stu-id="b2b2d-103">The list of browsers supported by Blazor in ASP.NET Core 5.0 has been updated accordingly.</span></span>

<span data-ttu-id="b2b2d-104">有关讨论，请参阅 GitHub 问题 [dotnet/aspnetcore#26475](https://github.com/dotnet/aspnetcore/issues/26475)。</span><span class="sxs-lookup"><span data-stu-id="b2b2d-104">For discussion, see GitHub issue [dotnet/aspnetcore#26475](https://github.com/dotnet/aspnetcore/issues/26475).</span></span>

#### <a name="version-introduced"></a><span data-ttu-id="b2b2d-105">引入的版本</span><span class="sxs-lookup"><span data-stu-id="b2b2d-105">Version introduced</span></span>

<span data-ttu-id="b2b2d-106">5.0</span><span class="sxs-lookup"><span data-stu-id="b2b2d-106">5.0</span></span>

#### <a name="old-behavior"></a><span data-ttu-id="b2b2d-107">旧行为</span><span class="sxs-lookup"><span data-stu-id="b2b2d-107">Old behavior</span></span>

<span data-ttu-id="b2b2d-108">Blazor Server 支持具有足够填充代码的 Microsoft Internet Explorer 11。</span><span class="sxs-lookup"><span data-stu-id="b2b2d-108">Blazor Server supports Microsoft Internet Explorer 11 with sufficient polyfills.</span></span> <span data-ttu-id="b2b2d-109">Blazor Server 和 Blazor WebAssembly 在[旧版 Microsoft Edge](https://support.microsoft.com/help/4533505/what-is-microsoft-edge-legacy) 中也能使用。</span><span class="sxs-lookup"><span data-stu-id="b2b2d-109">Blazor Server and Blazor WebAssembly are also functional in [Microsoft Edge Legacy](https://support.microsoft.com/help/4533505/what-is-microsoft-edge-legacy).</span></span>

#### <a name="new-behavior"></a><span data-ttu-id="b2b2d-110">新行为</span><span class="sxs-lookup"><span data-stu-id="b2b2d-110">New behavior</span></span>

<span data-ttu-id="b2b2d-111">Microsoft Internet Explorer 11 不支持 ASP.NET Core 5.0 中的 Blazor Server。</span><span class="sxs-lookup"><span data-stu-id="b2b2d-111">Blazor Server in ASP.NET Core 5.0 isn't supported with Microsoft Internet Explorer 11.</span></span> <span data-ttu-id="b2b2d-112">Blazor Server 和 Blazor WebAssembly 部分功能无法在旧版 Microsoft Edge 中使用。</span><span class="sxs-lookup"><span data-stu-id="b2b2d-112">Blazor Server and Blazor WebAssembly aren't fully functional in Microsoft Edge Legacy.</span></span>

#### <a name="reason-for-change"></a><span data-ttu-id="b2b2d-113">更改原因</span><span class="sxs-lookup"><span data-stu-id="b2b2d-113">Reason for change</span></span>

<span data-ttu-id="b2b2d-114">ASP.NET Core 5.0 中的 Blazor 新功能与这些旧版浏览器不兼容，因此减少了这些旧版浏览器的使用。</span><span class="sxs-lookup"><span data-stu-id="b2b2d-114">New Blazor features in ASP.NET Core 5.0 are incompatible with these older browsers, and use of these older browsers is diminishing.</span></span> <span data-ttu-id="b2b2d-115">有关详细信息，请参阅以下资源：</span><span class="sxs-lookup"><span data-stu-id="b2b2d-115">For more information, see the following resources:</span></span>

* [<span data-ttu-id="b2b2d-116">Windows 对旧版 Microsoft Edge 的支持也将在 2021 年 3 月 9 日终止</span><span class="sxs-lookup"><span data-stu-id="b2b2d-116">Windows support for Microsoft Edge Legacy is also ending on March 9, 2021</span></span>](https://support.microsoft.com/help/4533505/what-is-microsoft-edge-legacy)
* [<span data-ttu-id="b2b2d-117">Microsoft 365 的应用和服务将于 2021 年 8 月 17 日终止对 Microsoft Internet Explorer 11 的支持</span><span class="sxs-lookup"><span data-stu-id="b2b2d-117">Microsoft 365 apps and services will end support for Microsoft Internet Explorer 11 by August 17, 2021</span></span>](/lifecycle/announcements/m365-ie11-microsoft-edge-legacy)

#### <a name="recommended-action"></a><span data-ttu-id="b2b2d-118">建议的操作</span><span class="sxs-lookup"><span data-stu-id="b2b2d-118">Recommended action</span></span>

<span data-ttu-id="b2b2d-119">从这些旧版浏览器升级到[基于 Chromium 的新 Microsoft Edge](https://www.microsoft.com/edge)。</span><span class="sxs-lookup"><span data-stu-id="b2b2d-119">Upgrade from these older browsers to the [new, Chromium-based Microsoft Edge](https://www.microsoft.com/edge).</span></span> <span data-ttu-id="b2b2d-120">对于需要支持这些旧版浏览器的 Blazor 应用，请使用 ASP.NET Core 3.1。</span><span class="sxs-lookup"><span data-stu-id="b2b2d-120">For Blazor apps that need to support these older browsers, use ASP.NET Core 3.1.</span></span> <span data-ttu-id="b2b2d-121">ASP.NET Core 3.1 中的 Blazor 支持的浏览器列表尚未更改，记录在[支持的平台](/aspnet/core/blazor/supported-platforms?view=aspnetcore-3.1)中。</span><span class="sxs-lookup"><span data-stu-id="b2b2d-121">The supported browsers list for Blazor in ASP.NET Core 3.1 hasn't changed and is documented at [Supported platforms](/aspnet/core/blazor/supported-platforms?view=aspnetcore-3.1).</span></span>

#### <a name="category"></a><span data-ttu-id="b2b2d-122">类别</span><span class="sxs-lookup"><span data-stu-id="b2b2d-122">Category</span></span>

<span data-ttu-id="b2b2d-123">ASP.NET Core</span><span class="sxs-lookup"><span data-stu-id="b2b2d-123">ASP.NET Core</span></span>

#### <a name="affected-apis"></a><span data-ttu-id="b2b2d-124">受影响的 API</span><span class="sxs-lookup"><span data-stu-id="b2b2d-124">Affected APIs</span></span>

<span data-ttu-id="b2b2d-125">无</span><span class="sxs-lookup"><span data-stu-id="b2b2d-125">None</span></span>

<!--

#### Affected APIs

Not detectable via API analysis

-->