# ai-sdd-notes
Beginner-friendly notes, examples, and concepts for understanding Spec-Driven Development and building software with AI coding agents.
# SPEC-DRIVEN DEVELOPMENT (SDD)

```text
SPEC-DRIVEN DEVELOPMENT (SDD)
│
├── 1. WHY SDD?
│   │
│   ├── Problem: Vibe Coding
│   │   ├── Prompt → Code → Review → Fix → Repeat
│   │   ├── Works for small/simple tasks
│   │   └── Doesn't scale well
│   │
│   ├── Problems with Vibe Coding
│   │   ├── Context decay
│   │   ├── Technical debt
│   │   ├── Inconsistent architecture
│   │   ├── AI makes important decisions randomly
│   │   ├── Large/unmanageable changes
│   │   └── Cognitive debt
│   │
│   └── SDD Solution
│       ├── Define WHAT
│       ├── Define WHY
│       ├── Define constraints
│       ├── Define success criteria
│       └── Let agent determine much of HOW
│
│
├── 2. CORE PRINCIPLE
│   │
│   ├── Human = Architect / Driver
│   │   ├── Intent
│   │   ├── Product decisions
│   │   ├── Architecture decisions
│   │   ├── Trade-offs
│   │   └── Validation
│   │
│   ├── AI Agent = Muscle / Pair Programmer
│   │   ├── Explore code
│   │   ├── Create plans
│   │   ├── Write code
│   │   ├── Run tests
│   │   └── Review/validate
│   │
│   └── SPEC = Contract / Brain
│       ├── Human ↔ Human
│       ├── Human ↔ Agent
│       └── Project memory
│
│
├── 3. BENEFITS OF SPECS
│   │
│   ├── Control large changes
│   │   └── Small spec change → Large controlled code change
│   │
│   ├── Prevent context decay
│   │   └── Specs persist between sessions/agents
│   │
│   ├── Improve intent fidelity
│   │   └── Agent understands goals and constraints
│   │
│   ├── Reduce cognitive debt
│   │   └── Easier to understand what changed and why
│   │
│   └── Reduce AI fatigue
│       └── Smaller, manageable feature boundaries
│
│
├── 4. PROJECT CONSTITUTION
│   │
│   ├── Mission
│   │   ├── Why does the project exist?
│   │   ├── Vision
│   │   ├── Target audience
│   │   └── Scope
│   │
│   ├── Tech Stack
│   │   ├── Languages
│   │   ├── Frameworks
│   │   ├── Database
│   │   ├── Infrastructure
│   │   └── Engineering constraints
│   │
│   ├── Roadmap
│   │   ├── What are we building?
│   │   ├── Feature phases
│   │   └── Order/priorities
│   │
│   └── Living Document
│       ├── Can change
│       ├── Updated during replanning
│       └── Version controlled
│
│
├── 5. FEATURE DEVELOPMENT LOOP
│   │
│   ├── Step 1: Select Feature
│   │   └── Take next item from roadmap
│   │
│   ├── Step 2: Create Feature Spec
│   │   ├── Requirements
│   │   ├── User flows
│   │   ├── Constraints
│   │   ├── Plan
│   │   └── Validation criteria
│   │
│   ├── Step 3: Review Spec
│   │   ├── Human reviews
│   │   ├── Agent asks questions
│   │   ├── Correct assumptions
│   │   └── Resolve conflicts
│   │
│   ├── Step 4: Commit Spec
│   │   └── Version specification with Git
│   │
│   ├── Step 5: Implement
│   │   ├── Agent writes code
│   │   ├── Can work by task groups
│   │   └── Keep changes manageable
│   │
│   ├── Step 6: Human Review
│   │   ├── Does code match spec?
│   │   ├── Does feature work?
│   │   ├── Architecture correct?
│   │   └── Any unexpected changes?
│   │
│   ├── Step 7: Verify
│   │   ├── Run application
│   │   ├── Run tests
│   │   ├── Debug
│   │   ├── Review behavior
│   │   └── Agent/sub-agent review
│   │
│   ├── Step 8: Commit + Merge
│   │
│   └── Step 9: Replan
│       ├── Update Constitution
│       ├── Update Roadmap
│       ├── Update Specs
│       └── Improve workflow
│
│
├── 6. RIGHT LEVEL OF DETAIL
│   │
│   ├── Specify
│   │   ├── Goals
│   │   ├── Requirements
│   │   ├── Constraints
│   │   ├── User behavior
│   │   └── Success criteria
│   │
│   └── Don't over-specify
│       ├── Variable names
│       ├── Every function
│       ├── Every CSS class
│       └── Low-level implementation details
│
│       Rule:
│       "Tell the agent what it doesn't know,
│        let it figure out what it can."
│
│
├── 7. HUMAN-IN-THE-LOOP
│   │
│   ├── Agent asks questions
│   ├── Human makes decisions
│   ├── Agent creates spec
│   ├── Human reviews spec
│   ├── Agent implements
│   ├── Human reviews implementation
│   ├── Agent validates
│   └── Human accepts/rejects
│
│
├── 8. GIT + VERSIONING
│   │
│   ├── Feature branches
│   ├── Small commits
│   ├── Specs versioned with code
│   ├── Reviewable changes
│   ├── Merge feature
│   └── Track which specs produced changes
│
│
├── 9. REPLANNING
│   │
│   ├── After each feature
│   ├── Review what was learned
│   ├── Update Constitution
│   ├── Update Roadmap
│   ├── Update Feature Specs
│   ├── Improve testing strategy
│   ├── Improve SDD workflow
│   └── Decide next feature
│
│   ├── Small new requirement
│   │   └── Handle during replanning
│   │
│   └── Large new requirement
│       └── Add new roadmap feature
│
│
├── 10. TESTING & VALIDATION
│   │
│   ├── Application testing
│   ├── Automated tests
│   ├── Debugging
│   ├── Code review
│   ├── Spec validation
│   └── Deep agent/sub-agent review
│
│
├── 11. AI FATIGUE
│   │
│   ├── Problem
│   │   ├── Agent generates lots of code
│   │   ├── Huge diffs
│   │   └── Human review becomes exhausting
│   │
│   └── Solution
│       ├── Small features
│       ├── Small task groups
│       ├── Frequent commits
│       ├── Clean feature boundaries
│       ├── Clear agent context
│       └── High-level review
│
│
├── 12. COGNITIVE DEBT
│   │
│   ├── "What did the AI change?"
│   ├── "Why did it change it?"
│   ├── "What assumptions did it make?"
│   └── "Do I actually understand the code?"
│
│   SDD reduces this through:
│   ├── Specs
│   ├── Small changes
│   ├── Reviews
│   ├── Tests
│   └── Clear feature boundaries
│
│
├── 13. GREENFIELD
│   │
│   └── New Project
│       ├── Constitution
│       ├── Roadmap
│       ├── Feature Specs
│       ├── Implementation
│       └── Verification
│
│
├── 14. BROWNFIELD / LEGACY
│   │
│   ├── Existing codebase
│   ├── README
│   ├── TODOs
│   ├── Issues
│   ├── Existing documentation
│   └── Existing commits
│            ↓
│       Agent analyzes
│            ↓
│       Constitution
│            ↓
│       Roadmap
│            ↓
│       Normal SDD workflow
│
│   Key idea:
│   "Specs become the memory of the legacy project."
│
│
├── 15. MVP
│   │
│   ├── Strong Constitution
│   ├── Strong Feature Specs
│   ├── Larger implementation
│   ├── Agent builds MVP
│   ├── Validate against specs
│   └── Discover gaps → Replan
│
│
├── 16. AGENT SKILLS
│   │
│   ├── Reusable workflows
│   ├── Project-specific skills
│   ├── Global skills
│   ├── Progressive disclosure
│   ├── Skills can call other skills
│   └── Explicitly invoke when needed
│
│   Examples:
│   ├── Feature Spec Skill
│   ├── Validation Skill
│   ├── Changelog Skill
│   └── Research Skill
│
│
├── 17. MCP
│   │
│   └── Model Context Protocol
│       ├── External tools
│       ├── APIs
│       ├── Databases
│       └── External knowledge
│
│
├── 18. SKILLS + CLI
│   │
│   ├── Alternative/complement to MCP
│   ├── Agent
│   │    ↓
│   ├── Skill
│   │    ↓
│   └── CLI tool
│
│   └── Can sometimes be simpler
│       and use less context
│
│
├── 19. AGENTS.md
│   │
│   └── Project-level agent instructions
│       ├── Coding rules
│       ├── Architecture rules
│       ├── Testing rules
│       └── Constraints
│
│
├── 20. PLUGINS
│   │
│   ├── Agent extensions
│   ├── Can bundle capabilities
│   ├── Can be installed/updated
│   └── Security consideration
│       └── Only install trusted plugins
│
│
├── 21. ACP
│   │
│   └── Agent Client Protocol
│       ├── Agent ↔ IDE/Client
│       ├── Agent interoperability
│       ├── Plug-and-play agents
│       └── ACP Registry
│           ├── Discover agents
│           ├── Install agents
│           └── Connect agents
│
│
├── 22. AGENT INDEPENDENCE
│   │
│   ├── Claude Code
│   ├── Codex
│   ├── OpenCode
│   ├── Other agents
│   │
│   └── Same SDD workflow
│       └── Specs remain portable
│
│
├── 23. EXISTING SDD FRAMEWORKS
│   │
│   ├── GitHub Spec Kit
│   │   └── Constitution → Plan → Tasks → Implement
│   │
│   └── OpenSpec
│       └── Propose → Explore → Apply → Archive
│
│
└── 24. FINAL PHILOSOPHY
    │
    ├── Don't let AI guess important decisions
    ├── Capture decisions in specs
    ├── Keep specs and code synchronized
    ├── Let AI handle implementation
    ├── Keep humans responsible for intent
    ├── Review AI-generated changes
    ├── Validate before merging
    ├── Replan continuously
    └── Keep improving the workflow
```
