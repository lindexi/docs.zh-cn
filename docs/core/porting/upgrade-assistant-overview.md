---
title: .NET 升级助手概述
description: 简要介绍可帮助从 .NET Framework 进行迁移和将项目升级到 .NET 5 的 .NET 升级助手工具。
author: ardalis
ms.date: 02/25/2021
ms.openlocfilehash: bd1c904586d170d93b76ae058914adb334289f89
ms.sourcegitcommit: 42d436ebc2a7ee02fc1848c7742bc7d80e13fc2f
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "102108157"
---
# <a name="overview-of-the-net-upgrade-assistant"></a>.NET 升级助手概述

你可能有些应用当前正在 .NET Framework 上运行，而你想将它们移植到 .NET 5。 .NET 升级助手工具可帮助完成此过程。 本文提供以下内容：

* .NET 升级助手概述。
* 如何安装 .NET 升级助手。

## <a name="what-is-the-net-upgrade-assistant"></a>什么是 .NET 升级助手

.NET 升级助手是一种命令行工具，可在不同类型的 .NET Framework 应用上运行。 它旨在帮助将 .NET Framework 应用升级到 .NET 5。 大多数情况下，在运行该应用后，应用还需要执行多项操作来完成迁移。 该工具包含安装可帮助完成迁移的分析器。

该工具目前支持下列 .NET Framework 应用类型：

- .NET Framework Windows 窗体应用
- .NET Framework WPF 应用
- .NET Framework ASP.NET MVC 应用
- .NET Framework 控制台应用
- .NET Framework 类库

.NET 升级助手目前为预发行版，且正在频繁接收更新。 如果在使用该工具时发现问题，请在工具的 [GitHub 存储库](https://github.com/dotnet/upgrade-assistant)中进行报告。

## <a name="how-to-install-the-net-upgrade-assistant"></a>如何安装 .NET 升级助手

[入门教程](https://aka.ms/dotnet-upgrade-assistant-install)介绍了如何安装和使用 .NET 升级助手。

### <a name="prerequisites"></a>先决条件

1. 此工具使用 MSBuild 来处理项目文件。 请确保已安装最新版本的 MSBuild。 要做到这一点，一个简单的方法是[安装 Visual Studio 2019](https://visualstudio.microsoft.com/downloads/)。
1. 此工具依赖于 [try-convert](https://github.com/dotnet/try-convert)。 为使该工具正常运行，你必须安装 try-convert 来将项目文件转换为新的 SDK 样式。 如果已安装 try-convert，则转而可能需要更新它（原因是 upgrade-assistant 依赖于 0.7.212201 版或更高版本 ）
    1. 若要安装 try-convert：`dotnet tool install -g try-convert`
    1. 若要更新 try-convert：`dotnet tool update -g try-convert`

### <a name="installation-steps"></a>安装步骤

可运行以下命令将该工具安装为 .NET CLI 工具：

```dotnet
dotnet tool install -g upgrade-assistant
```

同样地，由于 .NET 升级助手是作为 .NET CLI 工具安装的，可运行以下命令来轻松更新它：

```dotnet
dotnet tool update -g upgrade-assistant
```

有关详细的安装说明，请查看项目的 [README](https://github.com/dotnet/upgrade-assistant)。

## <a name="see-also"></a>另请参阅

- [使用 .NET 升级助手将 WPF 应用升级到 .NET 5](upgrade-assistant-wpf-framework.md)
- [使用 .NET 升级助手将 Windows 窗体应用升级到 .NET 5](upgrade-assistant-winforms-framework.md)
- [使用 .NET 升级助手将 ASP.NET MVC 应用升级到 .NET 5](upgrade-assistant-aspnetmvc.md)
- [.NET 升级助手 GitHub 存储库](https://github.com/dotnet/upgrade-assistant)
