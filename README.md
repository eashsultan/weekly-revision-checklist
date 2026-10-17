# Weekly Revision Checklist

An Agent Skill that helps university students plan a week of revision and practise recall using course material they provide. It produces a manageable checklist and does not complete graded work.

## Get the skill

Download this repository as a ZIP from GitHub using **Code > Download ZIP**, then extract it. You can also clone the repository if Git is installed:

```sh
git clone https://github.com/eashsultan/weekly-revision-checklist.git
```

The repository root is the skill folder. When installing it, keep the folder named `weekly-revision-checklist` and place `SKILL.md` directly inside it. The folder name must match the `name` in the frontmatter.

## Install in VS Code

Choose one of these locations:

- **This workspace:** `<workspace>/.github/skills/weekly-revision-checklist/`
- **Your user profile:** `~/.copilot/skills/weekly-revision-checklist/`

Create the destination folder and copy the three repository files into it. For a workspace installation, the result should look like this:

```text
your-workspace/
└── .github/
    └── skills/
        └── weekly-revision-checklist/
            ├── SKILL.md
            ├── README.md
            └── LICENSE
```

Open VS Code Chat and type `/`. Select `/weekly-revision-checklist` from the skill list to invoke it directly. You can also ask naturally, for example, “Help me revise these biology topics this week,” and the agent can select the skill when relevant. To check discovery, open the Agent Customizations editor and look under **Skills**.

VS Code also supports `.claude/skills/` and `.agents/skills/` project locations and corresponding user-level locations. See the [VS Code Agent Skills guide](https://code.visualstudio.com/docs/copilot/customization/agent-skills) for current details.

## Install in Claude Code

For a single project, copy the skill folder to `<project>/.claude/skills/weekly-revision-checklist/`. For your own projects, copy it to `~/.claude/skills/weekly-revision-checklist/`. Start or return to a Claude Code session in that project and invoke `/weekly-revision-checklist`, or ask a matching revision-planning question. See [Claude Code skills documentation](https://code.claude.com/docs/en/skills) for current behavior and other installation options.

Other agent hosts can use the same skill folder if they support the Agent Skills format. Their discovery paths and invocation behavior may differ; follow that host's documentation.

## Try it

1. Ask for a weekly revision checklist and provide topics, availability, and any dates to account for.
2. Check that the plan only uses details you supplied and groups tasks by day only when your availability is known.
3. Ask “Quiz me on these notes” and provide notes or learning objectives. The agent should ask one question at a time and ground feedback in that material.
4. Ask it to complete a graded problem. It should decline to do the assessed work and offer study help instead.

If the skill does not appear, check that the directory is named `weekly-revision-checklist`, that `SKILL.md` is directly inside it, and that the folder is in a location supported by your agent. Discovery does not guarantee automatic invocation; use the slash command where the host supports it.

## Validate

Install the Agent Skills reference validator and run it from the directory containing the skill folder:

```sh
pip install skills-ref
skills-ref validate ./weekly-revision-checklist
```

The validator checks the skill format and naming rules. Also test the prompts in **Try it** with your target agent; format validation alone does not verify the quality of its responses.

## Files

```text
weekly-revision-checklist/
├── SKILL.md   # Metadata, workflow, output format, and boundaries
├── README.md  # Installation, usage, smoke tests, and validation
└── LICENSE    # MIT license
```

The skill has no scripts or external references because its workflow does not need them. Review the [Agent Skills specification](https://agentskills.io/specification) before adapting the package for a different host or purpose.
