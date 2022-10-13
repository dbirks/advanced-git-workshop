
# Scenarios

## Merge Conflict
`Dockerfile.merge-conflict`


## Push Conflict
`Dockerfile.push-conflict`

## Split Commit
`Dockerfile.split-commit`

Simulates having to split a set of unstaged changes into two (or more commits).

There are uncommitted changes in the `split.txt` file. 

Running `git diff` should look like this:
```
/git/git-workshop-clone # git diff
diff --git a/split.txt b/split.txt
index 3ea4248..3988358 100644
--- a/split.txt
+++ b/split.txt
@@ -1 +1,3 @@
+First line
 Middle line
+Last line
```

The goal is to make two separate commits:
* With just the `First line` change
* With just the `Second line` change
