**Artifex.Ghostscript.NET** - Crafted in C#, this is the most comprehensive managed wrapper library available for the Ghostscript library, which supports both 32-bit and 64-bit systems. Ghostscript itself serves as an interpreter for the PostScript language, as well as for PDF files, along with associated software and documentation.

In mid-2023, Ghostscript.NET underwent a significant transition as it was acquired by Artifex. However, after some time, we decided to part ways. As a result, I embarked on a new endeavor, creating a distinct library named Artifex.Ghostscript.NET. This independent project is now under my sole maintenance, ensuring its continued development and support.

[**NuGet: PM> Install-Package Ghostscript.NET**](http://nuget.org/packages/Artifex.Ghostscript.NET/)

**Contains**
* GhostscriptViewer - Render PDF, EPS, or multi-page PostScript files for on-screen viewing.
* GhostscriptRasterizer - Convert PDF, EPS, or multi-page PostScript files into various standard image formats.
* GhostscriptProcessor - Simplify the invocation of Ghostscript library with custom arguments/switches.
* GhostscriptInterpreter - Engage the PostScript interpreter functionality.

**Other features**
* Enables in-memory rasterization without the need for intermediate disk storage.
* Facilitates zooming in and out capabilities.
* Offers support for progressive updates.
* Permits the concurrent operation of multiple Ghostscript instances within a single process.
* Compatible with both 32-bit and 64-bit versions of the native Ghostscript library.

**Latest changes - 2023-10-07 - v.1.2.4.**
* Resolved the problem with PDF media calculations that was causing blank pages in the rendered PDF.
* When Ghostscript.NET parses comments like "%%BoundingBox", it expects line to end with either \n (Unix) or \r\n (Windows). This patch adds support for files generated on Apple devices where lines ends with '\r'.


