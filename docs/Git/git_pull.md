# git pull
Created вторник 16 Февраль 2021

usage: git pull [<options>] [<repository> [<refspec>...]]

-v, --verbose         be more verbose
-q, --quiet           be more quiet
--progress            force progress reporting
--recurse-submodules[=<on-demand>]
  control for recursive fetching of submodules

Options related to merging
-r, --rebase[=(false|true|merges|preserve|interactive)]
  incorporate changes by rebasing rather than merging
-n                    do not show a diffstat at the end of the merge
--stat                show a diffstat at the end of the merge
--log[=<n>]           add (at most <n>) entries from shortlog to merge commit message
--signoff[=...]       add Signed-off-by:
--squash              create a single commit instead of doing a merge
--commit              perform a commit if the merge succeeds (default)
--edit                edit message before committing
--cleanup <mode>      how to strip spaces and #comments from message
--ff                  allow fast-forward
--ff-only             abort if fast-forward is not possible
--verify-signatures   verify that the named commit has a valid GPG signature
--autostash           automatically stash/stash pop before and after
-s, --strategy <strategy>
  merge strategy to use
-X, --strategy-option <option=value>
  option for selected merge strategy
-S, --gpg-sign[=<key-id>]
  GPG sign commit
--allow-unrelated-histories
  allow merging unrelated histories

Options related to fetching
--all                 fetch from all remotes
-a, --append          append to .git/FETCH_HEAD instead of overwriting
--upload-pack <path>  path to upload pack on remote end
-f, --force           force overwrite of local branch
-t, --tags            fetch all tags and associated objects
-p, --prune           prune remote-tracking branches no longer on remote
-j, --jobs[=<n>]      number of submodules pulled in parallel
--dry-run             dry run
-k, --keep            keep downloaded pack
--depth <depth>       deepen history of shallow clone
--shallow-since <time>
  deepen history of shallow repository based on time
--shallow-exclude <revision>
  deepen history of shallow clone, excluding rev
--deepen <n>          deepen history of shallow clone
--unshallow           convert to a complete repository
--update-shallow      accept refs that update .git/shallow
--refmap <refmap>     specify fetch refmap
-o, --server-option <server-specific>
  option to transmit
-4, --ipv4            use IPv4 addresses only
-6, --ipv6            use IPv6 addresses only
--negotiation-tip <revision>
  report that we have only objects reachable from this object
--show-forced-updates
  check for forced-updates on all updated branches
--set-upstream        set upstream for git pull/fetch

