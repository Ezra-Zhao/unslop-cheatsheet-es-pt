# unslop 速查表 | unslop Cheatsheet | Guía rápida de unslop

> 📚 **Colección / Coleção**: esta hoja forma parte de [cheatsheets](https://github.com/Ezra-Zhao/cheatsheets) — 100 hojas de referencia en un solo repositorio. / Esta folha faz parte de [cheatsheets](https://github.com/Ezra-Zhao/cheatsheets) — 100 folhas de referência em um só repositório. ⭐

**紫渐变、三张一模一样的卡片、满屏发光——一眼就看出是 AI 做的。这一张教你的 agent 先认出这些毛病，再像设计师拿红笔改稿一样，一项一项改掉**

> 一页看懂 heydamir/unslop：一个给 Claude Code、Codex 与 Google Antigravity 用的设计 skill。它先审计一屏界面，把「AI 味」逐项列出来——紫色渐变、发光、emoji 标签、大喊式文案、间距不匀，都是原仓自己点名的毛病——再从产品本身定一个设计方向，然后一遍一遍地过：间距、颜色、图标、文案、字体、版式、细节、视觉与动效。改之前先给方向、让你把关；界面已经够好时，它会直说够好，只给小修建议，不硬找活干。

- 上游项目：[heydamir/unslop](https://github.com/heydamir/unslop)，作者 Damir Sokolovsky（2026-11-11 实测 14,374 ★ / 798 forks；0 个 release、29 个 commit；2026-10-29 建仓）
- 许可证：原仓为 **CC BY 4.0**——可商用，但必须署名 Damir Sokolovsky 并链回原仓；本仓照此办（署名见文末来源与声明）
- 宿主：Claude Code / Codex / Google Antigravity
- 本页结构：中文主文 → English → Español → Português

---

Apoyo y más: [GitHub Sponsors](https://github.com/sponsors/Ezra-Zhao) · [Gumroad — plantillas y cuadernos que uso](https://ezraflow28.gumroad.com) · [Ko-fi](https://ko-fi.com/ezra777zhao)

## 三个宿主，装法一行版

| 宿主 | 装法（原仓口径） |
|---|---|
| Claude Code | 把 skill 文件夹拷进 `~/.claude/skills`，或项目里的 `.claude/skills` |
| Codex | 用 skill-installer 一行装，或把文件夹拷进 `~/.agents/skills` |
| Google Antigravity | 把 skill 文件夹拷进 `~/.gemini/antigravity/skills` |

装法就是拷文件夹，没有安装包、没有版本发布（这件事的影响写在诚实标注区）。

## 用法三行卡

- **下令**：`/unslop` 加上要改的那一屏，或者一个网址。
- **也可以说人话**：直接用自然语言讲想改哪里，agent 自己会把这个 skill 调起来，不必每次敲命令。
- **能对线上站点下手**：只有链接、没有本地代码的站点，也能改（截图快照要另装东西，见下一张卡）。

## 改稿顺序卡：先审计、定方向，再九遍逐项过

顺序照原仓，别跳步：

0. **审计**：先把这一屏的 AI 味逐项列出来——紫色渐变、发光、emoji 标签、大喊式文案、间距不匀，看到什么列什么。
0.5 **定方向**：从产品本身定一个设计方向，**先拿给你把关**，你点头了再动手改。
1. 间距
2. 颜色
3. 图标
4. 文案
5. 字体
6. 版式
7. 细节
8. 视觉
9. 动效

一遍只管一件事，九遍过完再看整体。还有一条写在前头：界面已经够好时，它会直说够好、只给小修建议——不为了显得在干活而乱改。

## 可选件门槛卡（先说清，免得用时才发现缺东西、或者被扣费）

| 想要什么 | 还需要什么 |
|---|---|
| 给线上站点截快照 | 另装 Playwright 与 Chromium |
| 生成不到 10 秒的故事视频 | Playwright 与 Chromium 之外，还要 ffmpeg |
| hero 图用生图服务 | 可接 fal、Replicate 等付费服务。**每次付费生成之前，它会先把提示词亮出来问你**（原仓自述）——确认了才生成，不会悄悄扣你的费 |

## 诚实标注区

- **没有版本锚点**：0 个 release，装法是直接拷 skill 文件夹。自托管请自己锁一个 commit，别裸跟主干——上游哪天改了什么，你这边不会有任何提醒。
- **单人维护**：29 个 commit（2026-11-11 实测），迭代集中在作者一人身上。热度高，但维护结构就是这么薄，如实标注。
- **势头**：14,374 ★ / 798 forks（2026-11-11 原仓页实测，证据 A）；今日约 +986 星/天（第三方榜单口径，证据 B）。11 月 1 日它才约 4.1K 星，13 天涨到 14.4K，增速没掉下来。
- **权限提醒**：skill 是以你 agent 的权限运行的。装之前先打开 `SKILL.md` 从头读一遍再用（西语同类合集文章的通行提醒，证据 B）。
- **许可证是硬要求**：CC BY 4.0——署名 Damir Sokolovsky、链回原仓，是使用与再分发的前提，不是客气话。本页与本仓都照办。

---

## English (summary)

unslop (14,374 stars / 798 forks as of 2026-11-11; no releases, 29 commits, created 2026-10-29) is a design skill for Claude Code, Codex and Google Antigravity, written by Damir Sokolovsky and licensed CC BY 4.0 — attribution and a link back to the original repo are required, and this page complies. It first audits one screen and lists the "AI look" item by item — purple gradients, glow, emoji labels, shouty copy, uneven spacing are upstream's own examples — then derives a design direction from the product itself, shows you that direction for approval, and works through nine redline passes in order: spacing, color, icons, copy, typography, layout, details, visuals, motion. If the interface is already good, it says so and only suggests small fixes. Install is a folder copy: `~/.claude/skills` (or project `.claude/skills`) for Claude Code; the skill-installer one-liner or `~/.agents/skills` for Codex; `~/.gemini/antigravity/skills` for Antigravity. Use it with `/unslop` plus the screen or URL, or just describe the change in natural language and the agent picks the skill up; it can also work on a live site given only a link. Optional pieces: screenshotting live sites and generating story videos under 10 seconds need Playwright and Chromium (video also needs ffmpeg); hero images can use paid generation services such as fal or Replicate, and upstream states it shows you the prompt and asks before every paid generation, so nothing is charged quietly. Honest notes: with zero releases there is no version anchor — pin a commit if you self-host; the project is single-maintainer; and since a skill runs with your agent's permissions, read its `SKILL.md` fully before using it.

---

## Español (guía rápida — traducción de estudio, pendiente de revisión por un hablante nativo)

**Degradado morado, tres tarjetas idénticas, brillo por todas partes: se nota a la legua que lo hizo una IA. Esta guía enseña a tu agente a reconocer primero esos defectos y corregirlos después, uno por uno, como un diseñador con el bolígrafo rojo.**

unslop (14.374 estrellas / 798 forks a 11 de noviembre de 2026; sin releases, 29 commits) es un skill de diseño para Claude Code, Codex y Google Antigravity, creado por Damir Sokolovsky y publicado bajo licencia CC BY 4.0: se puede usar comercialmente, pero hay que atribuirlo a su autor y enlazar el repositorio original — esta página lo hace al final —. Su método: primero audita una pantalla y enumera el «sabor a IA» punto por punto — degradados morados, brillos, etiquetas con emoji, textos a gritos, espaciados irregulares, según la propia lista del repositorio original —; después define una dirección de diseño a partir del producto mismo, te la muestra para que la apruebes, y recién entonces corrige en nueve pasadas, en este orden: espaciado, color, iconos, texto, tipografía, composición, detalles, visual y movimiento. Si la interfaz ya está bien, lo dice sin rodeos y solo sugiere retoques menores.

Instalación, una línea por anfitrión: en Claude Code, copia la carpeta del skill a `~/.claude/skills` (o a `.claude/skills` dentro del proyecto); en Codex, instálalo con la línea de skill-installer o copia la carpeta a `~/.agents/skills`; en Google Antigravity, copia la carpeta a `~/.gemini/antigravity/skills`. Uso: `/unslop` seguido de la pantalla o la URL a corregir; también puedes pedirlo en lenguaje natural y el agente activa el skill solo; y puede trabajar sobre un sitio en línea del que solo tienes el enlace. Piezas opcionales, dichas de frente: para capturar instantáneas de sitios en línea y generar videos cortos de menos de 10 segundos hacen falta Playwright y Chromium (el video pide además ffmpeg); las imágenes principales pueden generarse con servicios pagos como fal o Replicate, y el propio repositorio aclara que antes de cada generación paga te muestra el prompt y te pide confirmación — no hay cargos silenciosos —. Notas honestas: sin releases no hay ancla de versión, así que si lo alojas tú mismo, fija un commit; es un proyecto de un solo mantenedor; y como un skill se ejecuta con los permisos de tu agente, abre el `SKILL.md` y léelo entero antes de usarlo.

---

## Português (guia rápido — tradução de estudo, aguardando revisão de um falante nativo)

**Gradiente roxo, três cartões idênticos, brilho em tudo: dá para ver de longe que foi uma IA que fez. Este guia ensina o seu agente a reconhecer primeiro esses defeitos e corrigi-los depois, um por um, como um designer com a caneta vermelha.**

O unslop (14.374 estrelas / 798 forks em 11 de novembro de 2026; sem releases, 29 commits) é um skill de design para Claude Code, Codex e Google Antigravity, criado por Damir Sokolovsky e publicado sob licença CC BY 4.0: pode ser usado comercialmente, mas é preciso atribuir a autoria e linkar o repositório original — esta página faz isso no final —. O método dele: primeiro audita uma tela e lista o «gosto de IA» item por item — gradientes roxos, brilhos, etiquetas com emoji, textos aos gritos, espaçamentos irregulares, pela lista do próprio repositório original —; depois define uma direção de design a partir do produto, mostra para você aprovar, e só então corrige em nove passadas, nesta ordem: espaçamento, cor, ícones, texto, tipografia, layout, detalhes, visual e movimento. Se a interface já está boa, ele diz isso sem enrolar e só sugere retoques menores.

Instalação, uma linha por hospedeiro: no Claude Code, copie a pasta do skill para `~/.claude/skills` (ou para `.claude/skills` dentro do projeto); no Codex, instale com a linha do skill-installer ou copie a pasta para `~/.agents/skills`; no Google Antigravity, copie a pasta para `~/.gemini/antigravity/skills`. Uso: `/unslop` seguido da tela ou da URL a corrigir; também dá para pedir em linguagem natural, e o agente ativa o skill sozinho; e ele consegue trabalhar sobre um site no ar do qual você só tem o link. Peças opcionais, ditas de frente: para capturar instantâneos de sites no ar e gerar vídeos curtos de menos de 10 segundos, são necessários Playwright e Chromium (o vídeo pede também o ffmpeg); as imagens principais podem ser geradas com serviços pagos como fal ou Replicate, e o próprio repositório esclarece que, antes de cada geração paga, ele mostra o prompt e pede a sua confirmação — sem cobranças silenciosas —. Notas honestas: sem releases não há âncora de versão, então, se você mesmo hospedar, fixe um commit; é um projeto de um único mantenedor; e como um skill roda com as permissões do seu agente, abra o `SKILL.md` e leia tudo antes de usar.

---

## 来源与声明

- 来源 / Source / Fuente / Fonte: [heydamir/unslop](https://github.com/heydamir/unslop)，作者 **Damir Sokolovsky**（2026-11-11 实测 14,374 ★ / 798 forks）。unslop 本体依 **CC BY 4.0** 发布，本仓依该许可证要求在此署名原作者并链回原仓；unslop 的名称、方法与文件归原作者所有。
- 本仓是个人学习整理：速查文字用我自己的话总结自上游公开文档，不搬运原文；装法与顺序以 2026-11-11 的上游 README 为准，星数以同日 GitHub 实测为准，上游迭代后请以官方文档为最终依据。
- 西语、葡语部分为学习译稿，待母语校对。Las secciones en español y portugués son traducciones de estudio pendientes de revisión nativa.
- License: 本仓原创文字 MIT © 2026 Guangyi Zhao；上游 unslop 内容依 CC BY 4.0（署名 Damir Sokolovsky，见上）。
