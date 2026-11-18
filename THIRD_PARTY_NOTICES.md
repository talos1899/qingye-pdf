# 第三方组件与许可

「轻页 PDF」的单个 HTML 文件中内联了以下第三方组件。完整许可文本位于本目录的 `third_party/` 中。

## PDF.js 3.11.174

- 版权：Mozilla Foundation 及 PDF.js 贡献者
- 许可：Apache License 2.0
- 许可全文：`third_party/LICENSE-pdfjs.txt`
- 项目：https://github.com/mozilla/pdf.js

## pdf-lib 1.17.1

- 版权：Copyright (c) 2019 Andrew Dillon
- 许可：MIT License
- 许可全文：`third_party/LICENSE-pdf-lib.md`
- 项目：https://github.com/Hopding/pdf-lib

## PDF.js CMap 数据

- 版权：Copyright 1990–2009 Adobe Systems Incorporated
- 许可：Adobe BSD-style 三条款许可
- 许可全文：`third_party/LICENSE-cmaps.txt`

## PDF.js 标准字体数据

### Foxit 字体（Fixed / Serif / Symbol / Dingbats）

- 版权：Copyright 2014 PDFium Authors
- 许可：BSD-style 三条款许可（PDFium）
- 许可全文：`third_party/LICENSE-foxit.txt`

### Liberation Sans

- 版权：Digitized data copyright (c) 2010 Google Corporation；Copyright (c) 2012 Red Hat, Inc.
- 许可：SIL Open Font License 1.1
- 许可全文：`third_party/LICENSE-liberation.txt`
- 项目：https://github.com/liberationfonts/liberation-fonts

## 说明

这些组件仅用于在浏览器本地解析、渲染和写出 PDF：

- PDF.js 负责把 PDF 页面渲染到画布，并提供 CMap 与标准字体回退数据。
- pdf-lib 负责在原始 PDF 上追加图片内容并下载新文件。
- 标准字体只在原 PDF 使用未嵌入的 Base 14 字体时作为回退，不会替换原文件里的字体。

发布、打包或转发时，请保留本文件和 `third_party/` 目录。
