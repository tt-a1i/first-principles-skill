# First Principles Thinking Skill

A Claude Code skill that provides systematic first principles thinking methodology for evaluating designs, challenging assumptions, and building solutions from fundamental truths.

## What is This?

This is a **skill** for [Claude Code](https://claude.ai/code) that enhances Claude's ability to analyze problems from first principles rather than relying on analogies or conventions.

## Installation

### Option 1: Copy to your skills directory

```bash
# Clone the repo
git clone https://github.com/YOUR_USERNAME/first-principles-skill.git

# Copy to Claude Code skills directory
cp -r first-principles-skill ~/.claude/plugins/superclaude/skills/first-principles
```

### Option 2: Symlink

```bash
git clone https://github.com/YOUR_USERNAME/first-principles-skill.git ~/skills/first-principles-skill
ln -s ~/skills/first-principles-skill ~/.claude/plugins/superclaude/skills/first-principles
```

## Usage

The skill triggers automatically when you use phrases like:

| Language | Trigger Phrases |
|----------|-----------------|
| English | "analyze from first principles", "think from scratch", "question this design", "is this the right approach", "challenge assumptions" |
| Chinese | "第一性原理", "从根本分析", "从零开始思考", "这个设计合理吗", "为什么要这样做", "有没有更好的方案" |

### Example

```
User: 用第一性原理分析一下我们是否应该采用微服务架构

Claude: [Applies first principles thinking methodology]

## First Principles Analysis: Microservices Architecture

### 1. Problem Essence
**Core problem:** Enable faster development and independent scaling
**Success criteria:** Deploy without full regression, scale components independently

### 2. Assumptions Challenged
| Assumption | Challenge | Verdict |
|------------|-----------|---------|
| Need microservices for modern apps | Do we have the team size? | Investigate |
...
```

## Structure

```
first-principles-skill/
├── SKILL.md                    # Main skill definition
├── README.md                   # This file
├── LICENSE                     # MIT License
├── references/
│   ├── software-examples.md    # Software engineering case studies
│   └── elon-musk-examples.md   # SpaceX/Tesla examples
└── examples/
    └── architecture-review.md  # Complete microservices analysis example
```

## Core Methodology

The skill follows a 5-phase process:

1. **Identify Problem Essence** - Strip away details to find the core problem
2. **Challenge Assumptions** - Question every assumption systematically
3. **Establish Ground Truths** - Identify irreducible facts
4. **Reason Upward** - Build solutions from fundamentals
5. **Validate Reasoning** - Ensure every decision traces to ground truths

## Output Format

The skill produces structured analysis:

```markdown
## First Principles Analysis: [Topic]

### 1. Problem Essence
### 2. Assumptions Challenged (table)
### 3. Ground Truths
### 4. Reasoning Chain
### 5. Conclusion
```

## Complementary Skills

This skill works well with:

- **5-Whys** - Dig deeper when assumptions surface
- **Trade-off Analysis** - Evaluate options against fundamentals
- **Pre-mortem** - Stress-test reasoning before implementation

## Contributing

Contributions welcome! Please feel free to submit issues or pull requests.

## License

MIT License - see [LICENSE](LICENSE) file.

## Author

Created for use with Claude Code's skill system.
