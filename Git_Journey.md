# My Git Mastery Challenge Journey

## Student Information
- Name: Supriya Palaparthi
- Student ID: 23A91A05H7
- Repository: https://github.com/palaparthisupriya/git-solved-23A91A05H7
- Date Started: 26-10-25
- Date Completed: 26-10-25

## Task Summary
Cloned instructor's repository with pre-built conflicts and resolved all 
merge conflicts across multiple branches using proper Git workflows.

## Commands Used

| Command | Times Used | Purpose |
|---------|------------|----------|
| git clone | 1 | Clone instructor's repository |
| git checkout | 20+ | Switch between branches |
| git branch | 10+ | View and manage branches |
| git merge | 2 | Merge dev and conflict-simulator into main |
| git add | 30+ | Stage resolved conflicts |
| git commit | 15+ | Commit resolved changes |
| git push | 10+ | Push to my repository |
| git fetch | 2 | Fetch updates from instructor |
| git pull | 1 | Pull updates |
| git stash | 2 | Save temporary work |
| git cherry-pick | 1 | Copy specific commit |
| git rebase | 1 | Rebase feature branch |
| git reset | 3 | Undo commits (soft/mixed/hard) |
| git revert | 1 | Safe undo |
| git tag | 2 | Create release tags |
| git status | 50+ | Check repository state |
| git log | 30+ | View history |
| git diff | 20+ | Compare changes |

## Conflicts Resolved

### Merge 1: main + dev (6 files)

#### Conflict 1: config/app-config.yaml
- **Issue**: Production used port 8080, development used 3000
- **Resolution**: Created unified config with environment-based settings
- **Strategy**: Keep production as default, add dev as optional
- **Difficulty**: Medium
- **Time**: 15 minutes

#### Conflict 2: config/database-config.json
- **Issue**: Different database hosts and SSL modes
- **Resolution**: Created separate profiles for production and development
- **Strategy**: Restructured JSON to support both environments
- **Difficulty**: Medium
- **Time**: 10 minutes

#### Conflict 3: scripts/deploy.sh
- **Issue**: Different deployment strategies (production vs docker-compose)
- **Resolution**: Added conditional logic based on DEPLOY_ENV variable
- **Strategy**: Made script handle both environments dynamically
- **Difficulty**: Hard
- **Time**: 20 minutes

#### Conflict 4: scripts/monitor.js
- **Issue**: Different monitoring intervals and log formats
- **Resolution**: Environment-based configuration object
- **Strategy**: Used process.env.NODE_ENV to determine behavior
- **Difficulty**: Medium
- **Time**: 15 minutes

#### Conflict 5: docs/architecture.md
- **Issue**: Different architectural descriptions
- **Resolution**: Merged both descriptions into comprehensive document
- **Strategy**: Created sections for each environment
- **Difficulty**: Easy
- **Time**: 10 minutes

#### Conflict 6: README.md
- **Issue**: Different feature lists and version numbers
- **Resolution**: Combined all features with clear environment labels
- **Strategy**: Organized features by category
- **Difficulty**: Easy
- **Time**: 10 minutes

### Merge 2: main + conflict-simulator (6 files)

###Conflict 1: config/app-config.yaml

-**Issue**: Experimental branch had AI features and multi-port server configuration, main had standard production settings.

-**Resolution**: Combined both configurations using environment-based keys (production, development, experimental).

--**Strategy**: Keep main production values as default; add experimental settings under a separate section.
-**Difficulty**: Hard

-**Time**: 20 minutes

###Conflict 2: config/database-config.json

-**Issue**: Experimental branch used distributed database with read replicas, main used single-node production DB.
-**Resolution**: Created a JSON structure supporting production, development, and experimental environments with separate connection settings.
-**Strategy**: Added AI optimization and read-replica options only under experimental.
-**Difficulty**: Hard
-**Time**: 15 minutes

###Conflict 3: scripts/deploy.sh

-**Issue**: Experimental deployment included multi-cloud, AI optimization, and canary deployment, conflicting with main’s production-only deployment script.
-**Resolution**: Added environment checks (DEPLOY_ENV) and implemented conditional logic for production vs experimental deployment.
-**Strategy**: Maintain backward compatibility while supporting experimental features.
-**Difficulty**: Hard
-**Time**: 25 minutes

###Conflict 4: scripts/monitor.js

-**Issue**: Experimental branch had AI monitoring and predictive scaling, main branch had standard interval-based monitoring.
-**Resolution**: Created environment-based configuration; AI features enabled only for experimental environment.
-**Strategy**: Preserve main monitoring behavior for production, extend experimental for AI-enhanced monitoring.
-**Difficulty**: Medium
-**Time**: 20 minutes

###Conflict 5: docs/architecture.md

-**Issue**: Experimental branch had AI/ML pipeline and multi-cloud architecture, main branch had standard microservices architecture.
-**Resolution**: Merged both versions into sections labeled Production, Development, and Experimental.
-**Strategy**: Clearly separate features for readability; indicate experimental features with ⚠️.
-**Difficulty**: Medium
-**Time**: 15 minutes

###Conflict 6: README.md
-**Issue**: Experimental branch had advanced features (AI integration, predictive scaling, multi-cloud orchestration) not present in main.
-**Resolution**: Combined legacy features with experimental features under clear environment headings.
-**Strategy**: Use Legacy Features and Cutting-Edge Features sections for clarity.
-**Difficulty**: Medium
-**Time**: 10 minutes

## Most Challenging Parts

1. **Understanding Conflict Markers**: Initially confused by `<<<<<<<`, `=======`, `>>>>>>>` symbols. Learned that HEAD is current branch and the other side is incoming changes.

2. **Deciding What to Keep**: Hardest part was choosing between conflicting code. Learned to read both versions completely before deciding.

3. **Complex Logic Conflicts**: deploy.sh had completely different logic. Had to understand both approaches before combining.

4. **Testing After Resolution**: Making sure resolved code actually worked was crucial.

## Key Learnings

### Technical Skills
- Mastered conflict resolution process
- Understood merge conflict markers
- Learned to use git diff effectively
- Practiced all major Git commands

### Best Practices
- Always read both sides of conflict before resolving
- Test resolved code before committing
- Write detailed merge commit messages
- Use git status frequently
- Commit atomically

### Git Workflow Insights
- Conflicts are normal, not errors
- Take time to understand both changes
- When in doubt, ask for clarification
- Document your resolution strategy
- Keep calm and read carefully

## Reflection
This challenge taught me that merge conflicts aren't scary - they're 
just Git asking "which version do you want?". The key is understanding 
what each side is trying to do before combining them. I now feel 
confident handling conflicts in real projects.

The hands-on practice with all Git commands (especially rebase and
 cherry-pick) was invaluable. I understand the difference between merge and rebase, 
and when to use each. Most importantly, I learned that git reflog is a lifesaver! 
given create git_journey.md
