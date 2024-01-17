#### Code quality enforcement
- Standardizing our code's format by using formatting tools and linters
- Reducing bugs and vulnerabilities in our code by introducing static code analysis tools
- Automating quality checks before pushing code to a repository
- Organizing our code and documenting it for clearer usage and reuse
- Creating a culture of learning through code reviews.

##### Constraints on development

- The focus on any company should be on trying to increase the throughput of the constrain
and protecting its time from being wasted at that stage. This is known as elevating the constraint.

- Static code analysis, code formatting, and code reviews are all examples of quality checks that

- Git hooks

```bash
#!/bin/bash
STAGED_GO_FILES=$(git diff --cached --name-only -- '*.go' )
if [[ "$STAGED_GO_FILES" = "" ]]; then
   echo "No Go files staged"
fi
else
  for file in $STAGED_GO_FILES; do
    gofmt -s -w $file
    git add $file
  done
fi
```

#### Summary

- Code quality checks can reduce bugs and standarize work
- Formatting can standarize a workspace and make it easier for newcomers to onboard.
- Static code analysis will check your code for known anti-patterns and ask you to fix them.
- Moving quality checks to the front of the pipeline can reduce wait time and catch bugs before deployment
- Constantly review and improve your development process to ensure the flow of the developer's work is smooth.

