---
publish: true
title: نمونه تستیار خوب LLMها، MCP
created: 0001-01-01
modified: 0001-01-01
published: 0001-01-01
socialDescription: توضیحاتی در زمینه اینکه MCP ها چی هستند و چه کمکی به ما میکنند
date: 0001-01-01
updated: 0001-01-01
unlisted: false
---

## 1 استفاده از MCP سرور ها در هوش مصنوعی

امروز با مفهوم جدیدی به نام MCP آشنا شدم، MCP روش استاندارد ارتباط گیری هوش مصنوعی با یک ابزار واقعی در سطح وب هستش، مثل یک استاندارد میمونه، مثلا ما برای وصل شدن به شبکه برق یک استاندارد داریم و اون پریز و دو شاخه برق هستش، MCP هم دقیقا همین طور کار میکنه یک استاندارد برای ایجاد ارتباط بین LLM ها با ابزار های دیگه.
تا اینجای کار فهمیدم که میتونم با cursor اتصال ساده بین LLM ها و MCP هارو داشته باشم. یکسری منابع هم پیدا کردم که میشه داخلشون MCP های خوبی پیدا کرد.

---

### 1.1 🧭 ۱. نقشه راه: پلتفرم‌های جامع MCP (General-Purpose Platforms)

این پلتفرم‌ها، موتورهای اصلی جستجو و کشف MCP سرورها هستند و برای شروع کار، بهترین گزینه به شمار می‌روند.

#### 1.1.1 🌍 رجیستری‌های عمومی (Public Registries)

- **[MCP Registry](https://registry.modelcontextprotocol.io)**: رجیستری رسمی و استاندارد پروتکل MCP که توسط خود پروتکل مدیریت می‌شود.
- **[MCP.so](https://mcp.so)**: یک دایرکتوری بزرگ و محبوب با ده‌ها هزار سرور و قابلیت جستجوی قوی.
- **[Smithery](https://smithery.ai)**: یکی از قدیمی‌ترین و معتبرترین رجیستری‌ها با بیش از ۷۰۰۰ قابلیت MCP.
- **[Glama MCP](https://glama.ai/mcp/servers)**: این رجیستری بر کیفیت سرورها تأکید دارد و بیش از ۳۵۰۰ سرور را با رتبه‌بندی عرضه می‌کند.
- **[Archestra MCP Catalog](https://archestra.ai/mcp-catalog)**: کاتالوگی با حدود ۹۰۰ سرور که با «امتیاز اعتماد آرکسترا» کیفیت آن‌ها را ارزیابی می‌کند.
- **[Portkey’s MCP Servers Directory](https://portkey.ai)**: دایرکتوری با بیش از ۴۰ سرور منبع‌باز.
- **[MCP Server Directories](https://dynomapper.com)**: فهرستی از خود دایرکتوری‌ها.

#### 1.1.2 🤝 رجیستری‌های ابری و سازمانی (Cloud & Enterprise Registries)

- **[PulseMCP](https://pulsemcp.com)**: یک دایرکتوری و مرکز خبری برای جامعه MCP که روزانه بیش از ۱۴,۰۰۰ سرور را به‌روز می‌کند.
- **[market.dev](https://explore.market.dev)**: یک دایرکتوری منبع‌باز از بیش از ۸۰۰۰ سرور MCP.
- **[Cursor Directory](https://cursor.directory/mcp)**: دایرکتوری تخصصی برای ویرایشگر Cursor.
- **[mcpdrop.com](https://mcpdrop.com)**: دایرکتوری ساده با تمرکز بر کشف سریع سرورها و دسته‌بندی آن‌ها (166 سرور در 12 دسته).

---

### 1.2 🛠️ ۲. قلب جامعه: مخازن گیت‌هاب (GitHub Repositories)

این مخازن توسط جامعه توسعه‌دهندگان ساخته و نگهداری می‌شوند و اغلب کامل‌ترین و به‌روزترین فهرست‌ها را ارائه می‌دهند.

#### 1.2.1 لیست‌های محبوب "Awesome"

- **[punkpeye/awesome-mcp-servers](https://github.com/punkpeye/awesome-mcp-servers)**: محبوب‌ترین و جامع‌ترین لیست Awesome که به عنوان منبع اصلی بسیاری از رجیستری‌ها استفاده می‌شود.
- **[wong2/awesome-mcp-servers](https://github.com/wong2/awesome-mcp-servers)**: این مخزن یکی از به‌روزترین لیست‌های Awesome است.
- **[tolkonepiu/best-of-mcp-servers](https://github.com/tolkonepiu/best-of-mcp-servers)**: یک رتبه‌بندی هفتگی از سرورها بر اساس معیارهای کیفیت گیت‌هاب و پکیج منیجرها.
- **[ever-works/awesome-mcp-servers](https://github.com/ever-works/awesome-mcp-servers)**: لیست انتخابی با جزئیات کامل که به عنوان وبسایت [mcpserver.works](https://mcpserver.works) نیز در دسترس است.
- **[salwad-basha-shaik/awesome-devops-mcp-servers-list](https://github.com/salwad-basha-shaik/awesome-devops-mcp-servers-list)**: لیست تخصصی برای سرورهای مرتبط با DevOps و زیرساخت.
- **[beriberikix/awesome-mcp-hardware](https://github.com/beriberikix/awesome-mcp-hardware)**: این مخزن روی سرورهای سخت‌افزاری و فیزیکی تمرکز دارد.

#### 1.2.2 مخازن تخصصی

- **[KshitijBhandari/awesome-mcp-server-directories](https://github.com/KshitijBhandari/awesome-mcp-server-directories)**: یک فهرست کامل از تمام دایرکتوری‌های MCP سرور. (لینک بررسی و فعال است).
- **[ADS39/Public-MCPs](https://github.com/ADS39/Public-MCPs)**: لیستی از MCPهای عمومی و آماده استفاده.
- **[199-mcp/mcp-servers-list](https://github.com/199-mcp/mcp-servers-list)**: مخزن منبع‌باز با فهرست جامعی از سرورها.
- **[salwad-basha-shaik/awesome-devops-mcp-servers-list](https://github.com/salwad-basha-shaik/awesome-devops-mcp-servers-list)**: همانطور که اشاره شد، این مخزن برای DevOps بسیار مفید است.
- **[habitoai/awesome-mcp-servers](https://github.com/habitoai/awesome-mcp-servers)**: لیست دیگری از سرورهای MCP و ابزارها.
- **[modelcontextprotocol/servers](https://github.com/modelcontextprotocol/servers)**: مخزن رسمی خود پروتکل MCP که شامل چند سرور مرجع و ارجاعات مفید است.

---

### 1.3 🎯 ۳. فهرست‌های تخصصی و شبکه‌های اجتماعی (Specialized & Social Platforms)

موتورهای جستجوی عمومی (مثل Google) محدودیت دارند؛ به همین دلیل شبکه‌های اجتماعی و پلتفرم‌های حرفه‌ای در اینجا به کمک می‌آیند.

- **Reddit:**
  - **[r/mcp](https://www.reddit.com/r/mcp)**: ساب‌ردیت اصلی MCP.
  - **[Top 5 Sources for finding MCP Servers](https://www.reddit.com/r/mcp/comments/1jgm0fp/top_5_sources_for_finding_mcp_servers)**: یک پست عالی که منابع مختلف را معرفی کرده.
  - **[GitHub MCP Registry Launches](https://www.reddit.com/r/mcp/comments/1fkdstb/github_mcp_registry_launches_another_week_another)**: بحث درباره یک رجیستری جدید.

- **LinkedIn:**
  - **[7 MCP Servers Every AI/ML/Data Engineer Should Try](https://www.linkedin.com/posts/pavan-belagatti_7-mcp-servers-every-ai-ml-data-engineer-activity-7301388869140889600-OI9X)**: پستی با معرفی ۷ سرور پرکاربرد.
  - **[10 MCP servers to supercharge your AI Agents](https://www.linkedin.com/posts/unwindai_10-mcp-servers-to-supercharge-your-ai-agents-activity-7312486599014772736-8IHp)**: ۱۰ سرور برای تقویت Agentهای هوش مصنوعی.

- **Hugging Face & Dev.to:**
  - **[My Personal Top MCP Servers — The Ultimate List](https://dev.to/flowstate/my-personal-top-mcp-servers-the-ultimate-list-5hfe)**: لیستی از بهترین سرورها توسط یک توسعه‌دهنده باتجربه.
  - **[The MCP Server Ecosystem 2026: Every Server Category You Need to Know](https://dev.to/jamesmurdza/the-mcp-server-ecosystem-2026-every-server-category-you-need-to-know-3pm0)**: توضیح کاملی از اکوسیستم MCP و دسته‌بندی سرورها.

---

### 1.4 🔧 ۴. ابزارهای کشف و CLI (Discovery & CLI Tools)

علاوه بر وبسایت‌ها، ابزارهای خط فرمان و پکیج‌های برنامه‌نویسی نیز برای یافتن MCP سرورها وجود دارند.

- **[mcp-server-find](https://pypi.org/project/mcp-server-find)**: یک MCP سرور که به Agentهای هوش مصنوعی کمک می‌کند MCP سرورهای دیگر را کشف کنند. داده‌ها را از رجیستری رسمی، Glama و Smithery جمع‌آوری می‌کند.
- **[mcphub](https://model-context-protocol.com)**: یک کلاینت خط فرمان برای نصب و مدیریت MCP سرورها از روی رجیستری npm.
- **[@mcpsearch/cli](https://www.npmjs.com/package/@mcpsearch/cli)**: یک ابزار رسمی برای کشف و نصب سرورها از طریق خط فرمان که پیکربندی آن‌ها را به ابزارهای کدنویسی هوش مصنوعی اضافه می‌کند.
- **[lazy-mcp](https://pypi.org/project/lazy-mcp)**: ابزاری برای ترکیب کردن چندین MCP سرور و مدیریت آن‌ها.
- **[Docker MCP Toolkit](https://docs.docker.com/desktop/mcp/toolkit/)**: ابزاری در Docker Desktop که به کاربران اجازه می‌دهد کاتالوگ MCP سرورهای Docker را مرور و آن‌ها را اجرا کنند.
- **[Apify MCP Directory Scraper](https://apify.com/bernardo/mcp-discovery-export)**: یک API برای اسکرپ کردن دایرکتوری‌های MCP و خروجی گرفتن از داده‌ها، با کتابخانه‌های Python و JavaScript.

---

تا اینجای کار میدونم که میشه با هر ابزاری که با LLM ها ارتباط میگیره به عنوان یک ایجنت و با MCP هم میتونه ارتباط بگیره یا ساپورت کنه این کار رو انجام دارد.
خیلی اتفاقی دنبال یک ایجنت میگشتم داخل VS Code که روی فیلتر زدم و بعد هم روی MCP و فهمیدم که خود VS Code یک مارکت پلیس هم برای MCP سرور ها داره و اونجا هم میشه دنبال MCP های مورد نیاز گشت.

الان باید 3 تا کار رو توی برنامه ام بذارم که همین الان تسک میکنمش چون دیدم باید وقت بیشتری براش بذارم

- [[وصل کردن مجدد کوپایلوت اوبزیدینم بعد از قطعی اینترنتها]]
- [[دانلود و نصب کرسر روی اوبونتو و تست کردنش]]
- [[نصب ایجنت های مختلف روی vscode و مقایسه شون]]

فعلا تا اینجای کار بمونه تا در آینده ببینم چی میتونم بهش اضافه کنم
