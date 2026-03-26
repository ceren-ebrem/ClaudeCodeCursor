# **Multimodal Generalists — Phase 1 Attempter Guidelines**

---

> ⚠️ **Image Collages Not Allowed**
> Images attached to prompts must NOT be collages created by combining multiple images (e.g., stitching screenshots together or arranging several photos into one image). A collage is allowed only if it already exists online as a single, originally published image and is attached as-is.

---

> ⚠️ **Image Sourcing**
> Images can be sourced from Google Images and academic papers, as long as they are available for commercial use (CC0 or CC-BY). Google Image Search is NOT fool-proof — always double-check that the image has the appropriate license and is not copyrighted. See [Image Guidelines](#image-guidelines) below.

---

## **Overview**

Welcome to Phase 1 of the Multimodal Generalists project.

This is a **multimodal** project focused on building evaluation data for general-purpose AI models. In Phase 1, your job is to:

1. **Write a natural, image-dependent prompt** in your assigned subdomain and difficulty level.
2. **Analyze six model responses** to confirm your prompt is complex enough to produce meaningful variance.
3. **Categorize the response landscape** by identifying distinct response types, a superior outlier, and an inferior/failure outlier.

**High-Level Outcomes:**

- Produce **image-dependent prompts** that reflect real-world user queries a general audience would genuinely ask.
- Prompts must be **open-ended enough** that different models respond in meaningfully different ways — in quality, depth, accuracy, or approach.
- Your prompt should **not** have a single short verifiable answer. It should invite a substantive response that can be evaluated along multiple dimensions.

---

## **🎯 Motivation**

Current state-of-the-art (SOTA) models are increasingly capable at text-only tasks. However, a significant gap remains in **multimodal reasoning for everyday contexts**: the ability to look at an image and respond to a natural, practical question the way a knowledgeable human assistant would.

Unlike specialized domains (medicine, law, engineering), generalist prompts reflect the actual queries that everyday users bring to AI systems — how-to questions, factual lookups, lifestyle advice, creative requests, and more. When an image is involved, the model must integrate visual content with world knowledge and practical reasoning.

We are building a dataset to measure and improve this capability. The goal is to create prompts where the image is genuinely essential and where the best models outperform weaker ones in ways that a careful human evaluator can identify and explain.

---

## **Prompt: Image Dependency**

### Core Requirement

The absolute requirement for every prompt is **image dependency**. If the problem can be answered using only the text, the prompt is **invalid**. The image must contribute information, context, or visual detail that is necessary to produce a complete, accurate response.

### Defining Validity

- **Valid:** The image contains specific visual content — an object, a scene, a label, a chart, a food item, a product, a situation — that the model must interpret in order to answer the prompt well.
- **Invalid:** The image is decorative, generic, or redundant. It adds nothing that could not be communicated in text.

### Domain-Specific Application Examples

Because this is a **Generalist** domain, prompts should feel like real questions a curious, everyday user would ask when sharing an image with an AI assistant.

| Subdomain | Example Prompt |
|---|---|
| **Knowledge & Factual Q&A** | "What is this architectural style and what period is it associated with?" (image: a building facade) |
| **How-To & Practical Advice** | "What's the best way to fix this? Any tips?" (image: a cracked tile or leaky pipe fitting) |
| **Health & Wellness** | "I found this plant in my backyard — is it safe to handle?" (image: a plant specimen) |
| **Finance & Consumer Decisions** | "Is this a good deal for what I see here?" (image: a product label or receipt) |
| **Education & Tutoring** | "Can you explain what this diagram is showing and why it matters?" (image: a textbook figure) |
| **Creative Writing & Storytelling** | "Write a short story inspired by the mood and setting of this image." (image: a landscape or street scene) |
| **Entertainment & Leisure** | "Can you identify this dish and suggest how I might recreate it at home?" (image: a restaurant meal) |
| **Editing & Rewriting** | "How would you improve the layout and text in this flyer?" (image: a hand-made event flyer) |
| **Personal & Relationships** | "I want to decorate this room differently — what would you suggest?" (image: a living room) |

---

## **Prompt Quality: What Makes a Good Generalist Prompt**

Generalist prompts are intentionally **open-ended**. Unlike STEM or professional prompts, they do not have a single correct answer. Instead, they should be rich enough that models can diverge meaningfully in how they respond.

### A Good Prompt:

- **Feels natural** — it reads like something a real user would actually type or say when sharing an image.
- **Requires the image** — the image provides context, detail, or specificity that makes the question answerable in a concrete way.
- **Invites substantive reasoning** — the model should need to interpret the image AND apply knowledge or judgment to respond well.
- **Has room for quality differentiation** — a stronger model will give a more accurate, nuanced, or practically useful answer than a weaker one.

### A Prompt is Invalid if:

- The image is not needed — the same question could be asked (and answered) without it.
- The prompt is so simple that any model gives essentially the same correct answer (no variance).
- The prompt asks only for extraction: "What color is the object in the image?" or "How many items are shown?"
- The prompt is unanswerable, offensive, time-dependent, or requires real-time web search.
- The prompt is vague to the point of meaninglessness — models cannot engage with it seriously.

---

## **Difficulty Levels**

All prompts must be written at your assigned difficulty level. Target distribution: **40% Easy, 40% Medium, 20% Hard.**

| Level | Definition |
|---|---|
| **Easy** | A clear, focused request with a single well-defined goal. The image adds obvious, interpretable context. A competent model can answer fully and correctly with minimal inference. |
| **Medium** | A multi-step or multi-layered request requiring synthesis of visual content with domain knowledge, practical judgment, or non-obvious reasoning. Some models will handle this better than others. |
| **Hard** | An ambiguous, nuanced, or complex scenario requiring deep real-world knowledge, subtle image interpretation, and careful reasoning. The best models will stand out significantly from weaker ones. |

---

## **Subdomains**

Assign your prompt to the most appropriate subdomain from the list below. Distribution across subdomains should reflect **real-world user query patterns** — do not artificially balance subdomains if the natural distribution favors certain topics.

- Knowledge & Factual Q&A
- How-To & Practical Advice
- Editing & Rewriting
- Health & Wellness
- Education & Tutoring
- Personal & Relationships
- Entertainment & Leisure
- Creative Writing & Storytelling
- Finance & Consumer Decisions

---

## **Image Guidelines** {#image-guidelines}

To ensure legal compliance and avoid copyright infringement, all images must strictly follow the guidelines below.

### ✅ Allowed Sources:

1. **Outlier Image Search**
2. **Google Image Search**
   - MUST be Creative Commons (CC0 or CC-BY) or Commercial & other licenses
   - MUST NOT have watermarks
3. **Pictures from CC0 or CC-BY papers or preprints**, including CC-BY-SA, CC-BY-3, CC-BY-4
   - ⚠️ CC-BY-NC and CC-BY-ND are NOT allowed
4. **Images taken or sourced yourself**
5. **Hand-drawn images** (pen & paper, Freeform, Apple Notes, Sketchbook)
6. **Screenshots of diagrams created in PowerPoint or Google Slides**
7. **Screenshots of Excel or Google Sheets**
8. **Python/R generated content**

Accepted formats: `.png`, `.jpeg`, `.jpg`

### 🚫 Disallowed Sources:

- Journal published figures outside CC0 or CC-BY licenses
- Images from CC-NC, CC-BY-ND, or other copyrighted sources
- Google Images results without a permissible license
- Images from Radiopaedia or AMBOSS

### 🚫 Other Restrictions:

- **Do NOT reuse images.** Each image may only be used for one prompt.
- **Do NOT create collages** by combining multiple images. A pre-existing published collage is allowed as-is.
- Do NOT modify copyrighted images (e.g., screenshotting a licensed paper and editing it in Paint). Copyrighted content remains protected in any form.

---

## **Response Analysis: Confirming Prompt Complexity**

After submitting your prompt, you will receive **six model responses**. Read all six carefully.

Your goal is to confirm that your prompt produces **significant variance** across the models — that is, the responses differ meaningfully in quality, depth, accuracy, approach, or level of engagement.

### A prompt passes this check if:

- At least 2–3 distinct types of responses are visible across the six models.
- At least one model responds notably better or worse than the others.
- The differences are not trivial (e.g., formatting differences or length differences alone do not count).

### A prompt fails this check if:

- All six models give essentially the same response with similar quality and content.
- The task was too simple — every model handles it fully and correctly.
- The task was unanswerable — every model fails or deflects in the same way.

**If your prompt fails the variance check, revise it and regenerate.** A more complex, image-dependent, or nuanced prompt will typically produce more variance.

---

## **Response Categorization & Outlier Audit**

Once your prompt passes the variance check, provide a qualitative map of the response landscape.

### 1. Distinct Response Types

Identify how many unique "types" of approaches are present across the six responses. Select a number from **2 to 6**.

A "type" is defined by a meaningfully different approach, framing, or level of engagement — not just surface differences in wording. For example:

- One type might give a practical step-by-step answer; another might give a general conceptual overview; a third might engage with the image deeply while others ignore key details.

### 2. Superior Outlier

Identify if any single response is **clearly and significantly better** than the rest across one or more of the following:

- Accuracy of information
- Depth and completeness of reasoning
- Correct and specific use of the image
- Practical usefulness to the user

If a superior outlier exists, select it and briefly explain what distinguishes it.

### 3. Inferior / Failure Outlier

Identify if any single response is **significantly worse** than the rest, including:

- Factual errors or hallucinations
- Failure to engage with the image
- Misinterpretation of the prompt
- Generic, evasive, or unhelpful output that does not address the user's actual question

If an inferior outlier exists, select it and briefly explain the failure.

> Note: A superior or inferior outlier does not have to exist. If the responses cluster into similar quality bands with no standout, mark accordingly.

---

## **📝 Complete Task Workflow**

| Step | Title | Description |
|---|---|---|
| **Step 1** | Select your subdomain and difficulty | Choose the subdomain from the approved list and confirm your assigned difficulty level (Easy / Medium / Hard). |
| **Step 2** | Find or create your image | Source an image that meets the image guidelines. The image should be specific enough to require genuine visual interpretation — not a generic stock photo. |
| **Step 3** | Write your prompt | Write a natural, image-dependent prompt in the style of a real user query. Confirm the image is required to answer it well. Confirm the prompt is open-ended enough to invite meaningful response variance. |
| **Step 4** | Indicate the image source | Record how the image was sourced or created. If from a CC0 or CC-BY paper, include the link. |
| **Step 5** | Submit and read model responses | Read all six model responses in full before forming any judgments. |
| **Step 6** | Variance check | Confirm that the six responses show significant variance in quality, approach, or content. If not, revise and resubmit. |
| **Step 7** | Categorize the response landscape | Select the number of distinct response types (2–6). Identify a superior outlier if one exists. Identify an inferior/failure outlier if one exists. Provide a brief explanation for each selection. |

---

## **📋 Task Checklist**

### ✅ Prompt Checklist

- [ ] Prompt is **image-dependent**: the image cannot be replaced by additional text
- [ ] Prompt is **natural**: it reads like a real user query, not a test question
- [ ] Prompt is **open-ended**: it invites a substantive response, not a single short answer
- [ ] Prompt is at the **correct difficulty level** for your assignment
- [ ] Prompt is assigned to the **correct subdomain**
- [ ] Prompt does **not** ask for simple extraction, counting, or identification alone
- [ ] Prompt is **not time-dependent** or reliant on web search
- [ ] Prompt is **not plagiarized** and is not logically equivalent to a previously submitted prompt
- [ ] Image follows all **image guidelines** (source, license, no collage, no reuse)
- [ ] Prompt is professionally written with no typos or grammatical errors

### ✅ Response Analysis Checklist

- [ ] All six model responses have been read in full
- [ ] Prompt produces **significant variance** across responses
- [ ] Number of distinct response types selected (2–6)
- [ ] Superior outlier identified or marked as absent, with explanation
- [ ] Inferior/failure outlier identified or marked as absent, with explanation
- [ ] Explanations reference **specific content** from the responses — not generic praise or criticism

---

## **Edge Cases**

### 1. Reusing Images
You may NOT reuse an image from one prompt for another, even if the prompt changes. Each image must correspond to exactly one prompt.

### 2. Time or Search Dependency
Prompts must be timeless. Do not write prompts that depend on current events, real-time data, or information that requires web search to answer.

### 3. Prompts That Are Too Open
A prompt like "What do you think of this image?" is too vague — it generates no meaningful variance because all models produce similarly generic responses. Prompts must have a specific ask that rewards domain knowledge, visual reasoning, or practical judgment.

### 4. Prompts Where Every Model Agrees
If all six models give essentially the same answer at similar quality, the prompt is too easy. Revise to increase complexity, specificity, or the degree to which the image is essential.

### 5. Prompts Where Every Model Fails
If all six models fail or deflect in the same way, the prompt may be unanswerable, too ambiguous, or violate guidelines (e.g., requires search, is time-dependent). Revise accordingly.
