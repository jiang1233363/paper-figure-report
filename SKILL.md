---
name: paper-figure-report
description: Prepare evidence-based, Feishu-ready research paper reports for a computer-science reader, especially biology foundation-model papers, with original figures and table screenshots explained in place.
---

# Paper figure report

Use this skill when the user asks for a detailed, copyable paper analysis or group-meeting report with figures and tables. Keep the paper's actual claims, data, and limitations separate from your own suggestions.

## Research and selection

- Read the primary paper, including methods, figure captions, tables, metric definitions, and relevant appendices. Check publication status and date. Verify unfamiliar biology terms with authoritative sources when needed.
- Select figures and tables that explain the question, architecture, dataset/evaluation, and main results. Prefer the paper's original figures. When the user asks for a table screenshot, crop the original paper table with its complete headers and rows; do not replace it with a transcribed Markdown table.
- Check that every reproduced image is readable and corresponds to the correct figure or table. Never invent or redraw a result as if it came from the paper.

## Writing for this user

- Write in Chinese for a computer-science reader. At first use, explain likely unfamiliar biological terms immediately in parentheses, using a short plain-language definition or CS analogy. For example, EC（按催化反应给酶编的四级标签） and CATH（按蛋白质三维结构域划分的四级标签）. Explain acronyms and biological evaluation metrics in the same way.
- In the report, use “论文” as the subject for methods, data, and results (e.g. “论文采用”, “论文构建”, “论文报告”); do not use “作者” as a stand-in for the paper.
- Cover research question, data, architecture, training objective, evaluation protocol, key experimental results, limitations, and research ideas worth borrowing. Spend space where the paper's figures and numbers justify it. Connect the analysis to a particular project only when the user asks.
- Place each image inline beside its discussion. Put its caption directly below the image in the form “图1：……” or “表1：……”. Explain the components or columns, then connect at least one concrete visual detail or number to the method or conclusion. Distinguish a paper result from your interpretation.
- Prefer direct observations such as “表2的 CATH L4 中，A 为 59.32%，B 为 86.44%” to generic advice or promotional conclusions. Do not use narrator phrases such as “读这张图时要注意” or “这张图告诉我们”.
- Make the report easy to paste into Feishu: do not use Markdown bold markers `**`; keep captions below images. Do not add source hyperlinks or bracketed citations such as `[论文图1](...)` or `[论文数据部分](...)` to the report. Give the paper title and publication details as plain text; provide reference links only if the user explicitly requests them. Keep the original figures and requested table screenshots embedded inline.
- Describe material caveats next to the relevant result: e.g. computational proxy versus laboratory validation, different input conditions, non-identical training settings, sample size, and possible data exposure. Do not turn a caveat into boilerplate.
- Title the final transfer section “借鉴”. Keep it to the two or three strongest reusable ideas, each stated in one or two sentences and tied to a figure or table result. Prefer a concrete modeling or evaluation choice over a broad checklist. Do not default to a named user project. Mark hypotheses as proposals rather than established results.

## Finish

Check every numeric claim against the paper and every caption against the image. Confirm that the final response contains the requested original images/table screenshots in position, with captions underneath, and no unexplained biology shorthand on first occurrence.
