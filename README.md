# GoogleTranslate.NET

### Version 1.1.0

A free and unlimited .NET Library for google translate without an API Key.

**This Library is only for Private, Open-Source, or Academic use.**

**Do not use this Library for commercial use!**

**For commercial use, please get an API key and use official Libraries. https://cloud.google.com/translate/docs/setup.**

# Usage

```cs
using GoogleTranslate;

GoogleTranslator translator = new ();
string targetLang = "eng";
string sourceLang = "de";
List<string> result = translator.Translate("Hi", targetLang, sourceLang);
// or
string result2 = translator.TranslateSingle("Hi", targetLang, sourceLang);
// you can also use automatic language detection
string result3 = translator.TranslateSingle("Hi", targetLang, "auto");
// you can can also cache Translations for less API calls
string result4 = translator.TranslateFromCacheOrNewSingle("Hi", targetLang, "auto");
```

# License

GoogleTranslate.NET is licensed under the MIT License. The terms are as follows:

```
MIT License

Copyright (c) 2022 3

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```