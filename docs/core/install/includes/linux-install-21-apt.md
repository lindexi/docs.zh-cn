---
ms.openlocfilehash: 164d7a8277cf985735b959c73eb87391944e795b
ms.sourcegitcommit: cdb295dd1db589ce5169ac9ff096f01fd0c2da9d
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/09/2020
ms.locfileid: "84602674"
---

### <a name="install-the-sdk"></a><span data-ttu-id="291ea-101">安装 SDK</span><span class="sxs-lookup"><span data-stu-id="291ea-101">Install the SDK</span></span>

<span data-ttu-id="291ea-102">.NET Core SDK 使你可以通过 .NET Core 开发应用。</span><span class="sxs-lookup"><span data-stu-id="291ea-102">.NET Core SDK allows you to develop apps with .NET Core.</span></span> <span data-ttu-id="291ea-103">如果安装 .NET Core SDK，则无需安装相应的运行时。</span><span class="sxs-lookup"><span data-stu-id="291ea-103">If you install .NET Core SDK, you don't need to install the corresponding runtime.</span></span> <span data-ttu-id="291ea-104">若要安装 .NET Core SDK，请运行以下命令：</span><span class="sxs-lookup"><span data-stu-id="291ea-104">To install .NET Core SDK, run the following commands:</span></span>

```bash
sudo apt-get update; \
  sudo apt-get install -y apt-transport-https && \
  sudo apt-get update && \
  sudo apt-get install -y dotnet-sdk-2.1
```

> [!IMPORTANT]
> <span data-ttu-id="291ea-105">如果收到类似于“找不到包 dotnet-sdk-2.1”的错误消息，请参阅 [APT 疑难解答](#apt-troubleshooting)部分。</span><span class="sxs-lookup"><span data-stu-id="291ea-105">If you receive an error message similar to **Unable to locate package dotnet-sdk-2.1**, see the [APT troubleshooting](#apt-troubleshooting) section.</span></span>

### <a name="install-the-runtime"></a><span data-ttu-id="291ea-106">安装运行时</span><span class="sxs-lookup"><span data-stu-id="291ea-106">Install the runtime</span></span>

<span data-ttu-id="291ea-107">.NET Core 运行时允许运行使用不随附运行时的 .NET Core 所开发的应用。</span><span class="sxs-lookup"><span data-stu-id="291ea-107">The .NET Core Runtime allows you to run apps that were made with .NET Core that didn't include the runtime.</span></span> <span data-ttu-id="291ea-108">以下命令安装 ASP.NET Core 运行时，这是与 .NET Core 最兼容的运行时。</span><span class="sxs-lookup"><span data-stu-id="291ea-108">The commands below install the ASP.NET Core Runtime, which is the most compatible runtime for .NET Core.</span></span> <span data-ttu-id="291ea-109">在终端中，运行以下命令。</span><span class="sxs-lookup"><span data-stu-id="291ea-109">In your terminal, run the following commands.</span></span>

```bash
sudo apt-get update; \
  sudo apt-get install -y apt-transport-https && \
  sudo apt-get update && \
  sudo apt-get install -y aspnetcore-runtime-2.1
```

> [!IMPORTANT]
> <span data-ttu-id="291ea-110">如果收到类似于“找不到包 aspnetcore-runtime-2.1”的错误消息，请参阅 [APT 疑难解答](#apt-troubleshooting)部分。</span><span class="sxs-lookup"><span data-stu-id="291ea-110">If you receive an error message similar to **Unable to locate package aspnetcore-runtime-2.1**, see the [APT troubleshooting](#apt-troubleshooting) section.</span></span>

<span data-ttu-id="291ea-111">作为 ASP.NET Core 运行时的一种替代方法，你可以安装不包含 ASP.NET Core 支持的 .NET Core 运行时：将上述命令中的 `aspnetcore-runtime-2.1` 替换为 `dotnet-runtime-2.1`。</span><span class="sxs-lookup"><span data-stu-id="291ea-111">As an alternative to the ASP.NET Core Runtime, you can install the .NET Core Runtime that doesn't include ASP.NET Core support: replace `aspnetcore-runtime-2.1` in the command above with `dotnet-runtime-2.1`.</span></span>

```bash
sudo apt-get install -y dotnet-runtime-2.1
```