# git merge
Created вторник 16 Февраль 2021

usage: git merge [<options>] [<commit>...]
   or: git merge --abort
   or: git merge --continue

-n                    do not show a diffstat at the end of the merge
--stat                show a diffstat at the end of the merge
--summary             (synonym to --stat)
--log[=<n>]           add (at most <n>) entries from shortlog to merge commit message
--squash              create a single commit instead of doing a merge
--commit              perform a commit if the merge succeeds (default)
-e, --edit            edit message before committing
--cleanup <mode>      how to strip spaces and #comments from message
--ff                  allow fast-forward (default)
--ff-only             abort if fast-forward is not possible
--rerere-autoupdate   update the index with reused conflict resolution if possible
--verify-signatures   verify that the named commit has a valid GPG signature
-s, --strategy <strategy>
  merge strategy to use
-X, --strategy-option <option=value>
  option for selected merge strategy
-m, --message <message>
  merge commit message (for a non-fast-forward merge)
-F, --file <path>     read message from file
-v, --verbose         be more verbose
-q, --quiet           be more quiet
--abort               abort the current in-progress merge
--quit                --abort but leave index and working tree alone
--continue            continue the current in-progress merge
--allow-unrelated-histories
  allow merging unrelated histories
--progress            force progress reporting
-S, --gpg-sign[=<key-id>]
  GPG sign commit
--autostash           automatically stash/stash pop before and after
--overwrite-ignore    update ignored files (default)
--signoff             add Signed-off-by:
--no-verify           bypass pre-merge-commit and commit-msg hooks

