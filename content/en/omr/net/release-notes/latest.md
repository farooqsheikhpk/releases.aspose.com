---
id: "aspose-omr-for-net-latest-release-notes"
slug: "latest"
weight: 1
date: "2024-01-22"
author: "Vladimir Lapin"
type: "repository"
layout: "release"
title: Latest release
description: A summary of recent changes, enhancements and bug fixes in the latest release of Aspose.OMR for .NET.
keywords:
- latest
- new
- release
- changelog
---

{{% alert color="primary" %}}
This article contains a summary of recent changes, enhancements and bug fixes in [**Aspose.OMR for .NET 24.1.0 (January 2024)**](https://www.nuget.org/packages/Aspose.OMR/24.1.0) release.
{{% /alert %}}

## What was changed

Key | Summary | Category
--- | ------- | --------
OMRNET&#8209;950 | Added support for plugins that extend the functionality of the core library. | New feature
_n/a_            | Simplified and streamlined the API by cleaning up deprecated methods. | Enhancement

## Public API changes and backwards compatibility

This section lists all public API changes introduced in **Aspose.OMR for .NET 24.1.0** that may affect the code of existing applications.

### Added public APIs:

The following public APIs have been added to Aspose.OMR for .NET 24.1.0:

#### `Aspose.OMR.Api.OmrEngine.AddPlugin()` method

This method extends the functionality of Aspose.OMR engine by incorporating additional features provided through a plugin.

### Updated public APIs:

_No changes_

### Removed public APIs:

The following public APIs have been removed from Aspose.OMR for .NET 24.1.0:

#### `Aspose.OMR.Api.TemplateProcessor.RecognizeMultiPageTemplate()` method

{{% alert color="warning" %}}
BACKWARD INCOMPATIBILITY!

This method has been deprecated in favor of the new API introduced in the [version 23.6.1](https://releases.aspose.com/omr/net/release-notes/2023/aspose-omr-for-net-23-6-1-release-notes/). Please update your code according to the recommendations below.
{{% /alert %}}

Use the universal [`Aspose.OMR.Api.TemplateProcessor.Recognize`](https://docs.aspose.com/omr/net/recognition/) method.

#### `Aspose.OMR.Api.TemplateProcessor.RecognizeImage()` methods

{{% alert color="warning" %}}
BACKWARD INCOMPATIBILITY!

This method has been deprecated in favor of the new API introduced in the [version 23.6.1](https://releases.aspose.com/omr/net/release-notes/2023/aspose-omr-for-net-23-6-1-release-notes/). Please update your code according to the recommendations below.
{{% /alert %}}

Use the universal [`Aspose.OMR.Api.TemplateProcessor.Recognize`](https://docs.aspose.com/omr/net/recognition/) method.

## Usage examples

See the examples below to learn more about the changes introduced in this release:

### Add handwriting recognition functionality

```csharp
// Initialize Aspose.OMR API
Aspose.OMR.Api.OmrEngine omrEngine = new Aspose.OMR.Api.OmrEngine();
// Activate recognition of handwritten text
engine.AddPlugin(new HandwritingPlugin());
```
