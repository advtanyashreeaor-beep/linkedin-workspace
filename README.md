# linkedin-workspace

A Claude Code workspace for LinkedIn content. The 12 LinkedIn skills from
[sergebulaev/linkedin-skills](https://github.com/sergebulaev/linkedin-skills) (v1.1.19, MIT —
see `.claude/LICENSE-linkedin-skills`) are vendored into `.claude/skills/`, so they load
automatically whenever this repo is opened in Claude Code — no plugin install needed:

| Skill | What it does |
|---|---|
| `linkedin-post-writer` | Draft a post from one of 20 hook formulas |
| `linkedin-content-planner` | 7-day content plan |
| `linkedin-comment-drafter` | Comment on / repost someone else's post |
| `linkedin-reply-handler` | Reply to one comment or sweep a whole thread |
| `linkedin-humanizer` | Remove AI tells; `--mode audit` / `--mode profile` |
| `linkedin-repurposer` | Turn a tweet, video, blog or newsletter into a LinkedIn post |
| `linkedin-hook-extractor` | Reverse-engineer a viral post's hook |
| `linkedin-profile-optimizer` | Audit and rewrite your profile |
| `linkedin-interviewer` | Build a Story Bank of raw material |
| `linkedin-engager-analytics` | Segment who liked/commented on a post (Apify) |
| `linkedin-thread-monitor` | Track author replies to your comments (Apify) |
| `linkedin-employee-advocacy` | Run a team advocacy program |

Supporting files live alongside them in `.claude/` (`references/`, `lib/`, `scripts/`,
`requirements.txt`). Skills that publish or scrape need API keys: copy `.claude/.env.example`
to `.claude/.env` and fill it in (never commit it). Python helpers: `pip install -r .claude/requirements.txt`.
