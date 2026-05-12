---
name: x-research
description: use this when you wanna do deep research on twitter/x.
---

# x-research

## setup

Check if `twitter` cli is installed and configured properly. You can install it from 
https://github.com/public-clis/twitter-cli

use /twitter-cli skill to make sure twitter cli is working properly.

If the user doesn't have uv to install twitter cli, you can install from this source
https://docs.astral.sh/uv/getting-started/installation/

Install twitter-cli skill from the skill store.

```
npx skills add jackwener/twitter-cli
```

## keep in mind
- twiter or x are same and can be used interchangeably in the context of this skill.

## When to use

Use this skill when you wanna do deep research on twitter/x. 

## Instructions

1. Get the current date before starting research.
   Use it to judge recency, spot outdated claims, and anchor any time-sensitive findings.

2. Clarify the research target.
   Identify the topic, people, companies, products, error messages, hashtags, keywords, date ranges, and versions that matter.

3. Generate multiple query variations before searching.
   Include:
   - Exact phrases in quotes when relevant
   - Common abbreviations and full names
   - Alternate terminology used by beginners and experts
   - Product names, version numbers, and environment details
   - Possible misspellings or shorthand
   - Searches for both the problem and likely solutions

4. Search using twitter cli
   - search for generated queries using twitter cli
   - search for accounts's tweets using twitter cli
   - search for account's replies, highlights, threads using twitter cli
   - if the tweet is a thread i.e other tweets are linked to it, read the few more levels of the thread to get more context and details.
   - refer to "Some Twitter specific flows to use" below for more details

5. Prioritize sources by signal, not just popularity.
   Prefer:
   - Firsthand report
   - Maintainer or official account statements
   - Tweets with concrete evidence, code, screenshots, or repro details
   - Threads with meaningful discussion in replies
   Treat vague, engagement-driven, or unsupported claims as lower confidence.

6. Read beyond the top tweets.
   Valuable details are often buried in:
   - Reply chains
   - Quote tweets
   - Follow-up corrections
   - Later updates from the original author

7. Track patterns across multiple tweets.
   Note:
   - Repeated symptoms or claims
   - Agreement across independent authors
   - Conflicting explanations
   - Whether newer tweets supersede older ones

8. Capture evidence carefully.
   For each useful finding, record:
   - A short summary of the claim
   - The author
   - The date
   - Relevant versions or environment details
   - A direct link to the tweet or thread
   - Whether the claim is firsthand, official, or secondhand

10. Watch for outdated or superseded information.
    Always check whether:
    - The issue was later resolved
    - The guidance only applied to an older version
    - A later thread corrected the earlier advice

11. Synthesize findings into a concise summary first.
    Start with 2 to 3 sentences covering:
    - What the strongest evidence suggests
    - What remains uncertain
    - The most promising next step or conclusion

12. Organize the detailed findings as a clean list.
    For each major finding or approach, include:
    - What it says
    - Why it matters
    - Confidence level
    - Tradeoffs or caveats
    - Direct source links
    - Since you're already reading tweets while mentioning direct links add markdown blockquote to quote the whole tweet and link before so users dont have to open twitter to see the whole tweet. 

13. Highlight conflicts instead of flattening them.
    If sources disagree, explain:
    - What the disagreement is
    - Which side has stronger evidence
    - What would need verification

14. End with a short self-check before presenting results.
    Confirm:
    - The search covered diverse query variations
    - The findings are current enough for the question
    - The strongest claims are backed by direct sources
    - The final output gives the user actionable next steps

### Some Twitter specific flows to use:
save-report: 
-> write the research output in a markdown file

#### Keyword based research
based on the user's query 
-> propose a plan and refine by asking questions 
-> think of keywords based on the research
-> search the top tweets on that keyword & users who post about that topic.
-> save-report

#### User's feed based research
Feed based research
based on user's query 
-> keep searching the users's feed's tweets
-> save-report


#### Twitter account research
based on users query 
-> Check the tweets of accounts given by user, 
-> browse tweets, highlights, replies
-> find patterns and insights
-> save-report

#### User's Account research
based on users query
-> Check user's tweets, highlights, replies.
