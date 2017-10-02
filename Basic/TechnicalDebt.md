# Concrete things you can do about your technical debt

1. Organize a lunch-and-learn with your team to introduce the concept of technical debt. Illustrate it with examples from your own projects, if possible.
2. Create a category “TechDebt” in your issue tracking system, distinct from defects, or new features. Point at the specific artifacts involved.
3. Standardize on one single form of “Fix me” or “Fix me later” comment in the source code to mark places that should be revised and improved later. They will be easier to spot with a tool.
4. Acquire and deploy in your development environment a static code analyser to detect code-level “code smells”. (Do not panic in front of the large number of positive warnings).
5. Prioritize technical debt items to fix or refactor, by doing them first in the parts of your code that are the most actively modified, leaving aside or for later the parts that are never touched.
6. Organize small 1-hour brainstorming sessions around the question: “What design decision did we make in the past that we regret now because it is costing us much?” or “If we had to do it again, what should have we done?” This is not a blame game, or a whining session; just identify high level structural issues, the key design decisions from the past that have turned to technical debt today.
7. For identified tech debt items, give not only estimates of the cost to “reimburse” them or refactor them (in staff effort), but also estimate of the cost to not reimburse them: how much it drags the progress now. At least describe qualitatively the impact on productivity or quality. This can be assisted by tools from your development environment, to look at code churn, and effort spent.
8. At each development cycle, try to constantly reduce some of the technical debt by explicitly bringing some tech debt items into your iteration or sprint backlog.
9. Refine in your issue tracker the TechDebt category into at least 2 subcategories: simple, localized, code-level debt, and wide ranging, structural or architectural debt.
10. For your major kinds of technical debt, identify the root cause –schedule pressure, process or lack of process, people availability or turn over, knowledge or lack of knowledge, tool or lack of tool, change of strategy or objectives–  and plan specific actions to address these root causes, or mitigate their effect.
11. Acquire and deploy a tool that will give you hints about structural issues in your code: dependency analysis.
12. Develop an approach for systematic regression testing, so that fixing technical debt items does not run you in the risk of breaking the code. (Counter the “It is not really broken, so I won’t fix it.”)
13. If you are actively managing risks, consider bringing some major tech debt items in your list of risks.
