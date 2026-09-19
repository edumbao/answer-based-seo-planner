# Answer-Based SEO Article Planner

A small public SEO planning tool that turns one search question into a structured article-planning prompt.

**Live tool:** https://edumbao.github.io/answer-based-seo-planner/

**Repository:** https://github.com/edumbao/answer-based-seo-planner
## Project status

**Working learning project**

The current version is intentionally simple. It is not a keyword research platform, SERP analyzer, or full content-generation system. It helps organize the direction of an article before drafting.

## Why I built it

I work in SEO and content, and I often start articles by trying to answer a specific search question clearly.

The problem is that a question alone is usually not enough to create a useful brief. I still need to think about:

- who the article is for
- the main angle or point of view
- an example or scenario
- the next action I want the reader to take

I built this tool to make that planning step easier to repeat.

It also gave me a small project where I could practice HTML, CSS, JavaScript, GitHub Pages, and analytics while working on a problem connected to my day-to-day content work.

## What the tool does

The planner asks for five inputs:

1. **Article question**
2. **Main audience**
3. **Main angle or point of view**
4. **Example or scenario**
5. **Call to action**

It then turns those inputs into a copy-ready prompt for an initial article review draft.

The generated prompt includes basic writing instructions such as:

- answer the main question clearly
- keep the structure focused
- use the search question as the basis for the article
- use short paragraphs
- add examples where they help
- treat the output as an initial review draft rather than a finished article

## How it works

```text
Search question
      ↓
Audience
      ↓
Angle
      ↓
Example
      ↓
Call to action
      ↓
Structured planning prompt
```

The tool runs as a static webpage and does not require a login.

## Tech stack

- HTML
- CSS
- Vanilla JavaScript
- GitHub Pages
- Google Analytics

The project is intentionally lightweight. I did not use a framework or database because the current workflow does not need one.

## Current features

- Article-question input
- Audience field
- Angle / point-of-view field
- Example or scenario field
- CTA field
- Prompt generation
- Copy-to-clipboard
- Clear form
- Share and embed options
- Google Analytics event tracking for prompt generation
- Responsive layout

## What it does not do

The current version does **not**:

- perform keyword research
- retrieve live SERP data
- measure search volume
- score search intent
- check competitors
- generate a final publish-ready article
- replace editorial review

I think keeping these boundaries clear is important because this is a planning utility, not a full SEO platform.

## Run it locally

Clone the repository:

```bash
git clone https://github.com/edumbao/answer-based-seo-planner.git
```

Move into the project:

```bash
cd answer-based-seo-planner
```

Because the project is a static site, you can either open `index.html` directly in a browser or serve it locally.

For example, with Python:

```bash
python -m http.server 8000
```

Then open:

```text
http://localhost:8000/
```

## Project structure

```text
answer-based-seo-planner/
├── index.html
├── LICENSE
└── README.md
```

The current application is contained in a single `index.html` file, including the page structure, styles, and JavaScript.

## What worked

A few parts of the project worked well for what I wanted to test:

- I was able to turn a repeated planning process into a working browser tool.
- The form keeps the planning workflow focused on a small set of inputs.
- The generated output is easy to copy into another writing workflow.
- The project works without a backend or account system.
- I added analytics so I can track when people use the Generate button.

## What confused me or still needs work

The tool is functional, but there are still things I want to improve.

### Input validation

The current version can generate a prompt even when important fields are empty. I want to require at least an article question and give clearer feedback when it is missing.

### Copy feedback

The Copy button currently uses a browser alert. I would like to replace that with a smaller inline confirmation message.

### Sharing options

The current sharing menu has more options than the core tool probably needs. I may reduce this to a simpler set of sharing actions.

### Project documentation

The first version of this README was only two lines long. Improving the documentation is part of the project because I want the repository to explain not just what the tool does, but why I built it and what I learned.

## What I learned

This project reinforced a few things for me:

- A useful tool does not have to be technically large.
- A repeated content task can be a good starting point for learning code.
- HTML, CSS, and JavaScript are enough for many small workflow tools.
- Clear boundaries matter. A planning tool should not pretend to be a complete SEO platform.
- Documentation is part of the project, not something to add only after the code is finished.
- Analytics can help me understand whether people actually use the tool instead of judging it only by page visits.

## How this connects to my SEO and content work

The project came directly from the way I think about article planning.

Instead of starting with a broad topic and immediately drafting, I prefer to clarify:

- the question being answered
- the reader
- the angle
- the example
- the next step

Turning that process into a small tool helped me make the workflow easier to repeat while also giving me hands-on practice with web development and technical documentation.

## What I want to try next

The next improvements I am considering are:

1. Require an article question before generating a prompt.
2. Improve copy-to-clipboard feedback.
3. Simplify the sharing interface.
4. Add a clearer distinction between a weak article question and a stronger one.
5. Keep documenting the project as I make small changes.

I do not want to add features just to make the project look larger. The goal is to keep it useful, understandable, and connected to a real content workflow.

## About this project

I am a content and SEO professional learning more about GitHub, APIs, automation, and coding by building small tools around problems I encounter in my work.

This repository is part of that learning process.

More projects and build notes: https://edumbao.com/lab/

## License

See the `LICENSE` file in this repository for the current license terms.
