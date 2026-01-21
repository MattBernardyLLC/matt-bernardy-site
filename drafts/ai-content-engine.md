# How I Built an AI Content Engine in Claude Code

I just built a system that takes me from interview to published blog post. Not a template. Not a prompt I copy-paste. A system that remembers how I want to write and gets better every time I use it.

Claude Code lets you create persistent skills, markdown files that define how you want the AI to behave for specific tasks. Unlike chat prompts that disappear, skills stay. They accumulate. They become institutional knowledge for your AI assistant.

## The Situation

I wanted to write more. Specifically, I wanted to turn the marketing stories in my head into blog posts that could support my job search. But every time I sat down to write, I hit the same walls: blank page paralysis, inconsistent voice, forgetting SEO basics, manual publishing steps that broke my flow.

I'd been using AI to help with writing, but it was always one-off. Paste a prompt, get output, manually fix everything, forget what I fixed, repeat the same mistakes next time.

What I needed was a way to encode my preferences once and have them persist.

## What I Built

The system has five parts that work together.

**Voice Interview (Custom GPT)**

I built an AI interviewer in ChatGPT that knows marketing benchmarks and pushes past vague answers. When I say "we improved performance," it asks "by how much?" When I mention a campaign, it asks what went wrong. It pulls the real stories out of me through conversation, then consolidates the transcript into structured material I can hand off to the next step.

**Narrative Copywriting Skill**

This is a Claude Code skill that takes interview transcripts or topic briefs and writes in my voice. I spent some time teaching it how I actually want to sound. No em dashes. No "full stop" for emphasis. Frame problems as design gaps, not incompetence. Lead titles with business metrics. End with customer impact, not business jargon.

Every correction I made during editing became a permanent rule. The skill file grew as I refined it.

**Executive Reviewer Skill**

Reads drafts through a CEO's eyes. Does this position me as a business leader or a marketing tactician? Are the metrics ones a board would care about? It flags places where I could be more accurate and add nuance. For case studies and thought leadership, this catches the difference between sounding like a marketer and sounding like someone who belongs at the leadership table.

**SEO Review Skill**

Checks title length, meta description, slug structure, header hierarchy, internal linking opportunities. Returns specific suggestions with character counts and alternatives, not vague advice about "optimizing for search."

**Publish Skill**

Converts the approved markdown to HTML using my site's template, updates the blog index, updates the sitemap, commits to git, and pushes to production. One command. The post is live.

## What Happened

I used this system to write [my first case study](/blog/swing-demand-gen-system). The interview surfaced stories I'd forgotten. The copywriting skill produced a draft that was 80% there. The executive reviewer caught places where I was underselling the business impact. SEO review tightened the title and meta description.

The whole process felt like working with a team that already knew my preferences. No re-explaining. No starting from scratch.

The skill files are version controlled. When I refine something, it sticks. The next post will be better because this post taught the system something.

The initial skills took a couple hours to build. But I refined them throughout the process of writing and editing the first post. Every time I corrected something, I added the rule to the skill. By the end, the system knew my preferences better than I could have specified upfront.

## What I'd Do Differently

I'd build the voice interview GPT earlier. The quality of the output depends entirely on the quality of the input. Garbage in, garbage out. The interview step is where the real stories surface. Everything downstream is just formatting and polish.

I'd also create separate reviewer personas faster. The executive reviewer works for case studies. But for AI tinkering posts like this one, I need a different lens. That's next.

## The Takeaway

This is what AI for marketers actually looks like. Not replacing the thinking. Encoding the thinking so you don't have to repeat it.

The system remembers what I taught it. It applies those lessons consistently. And it frees me to focus on the parts that actually require judgment: what stories to tell, what points to make, what to cut.

The post is live. The system is ready for the next one.

---
**Category:** AI Tinkering
**Meta description:** I built an AI content system in Claude Code that takes me from interview to published blog post. Here's exactly how it works and what I learned building it.
**Slug:** /blog/ai-content-engine
