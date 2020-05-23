# Steps

This is the step by step demo so that we can reproduce this live with Students on Sunday.

The first commit in this repository is a README with an introduction.
There are three issue that are unassigned at the moment:

* Add bio for Evan (#1)
* Add bio for Stéphane (#2)
* Add bio for Joel (#3)

We can spend a bit of time discussing what issues and milestones are.

# Stéphane prepares his bio, Even creates a conflict
Stéphane creates a branch to add his bio on the first commit. While he's doing
that, Even [pushes a commit with his own bio](https://github.com/snicoll-scratches/hyf-coach-bios/commit/07fc38aea47fc565f780eff0c993a11b2818a08e) on `master`, Closing #1.

I have no idea that Evan did that.

# Stéphane wants to merge his branch
Because I am behind, I can merge my branch locally just fine. However if I try to push it, I get this:

```
To https://github.com/snicoll-scratches/hyf-coach-bios.git
 ! [rejected]        master -> master (non-fast-forward)
error: failed to push some refs to 'https://github.com/snicoll-scratches/hyf-coach-bios.git'
hint: Updates were rejected because the tip of your current branch is behind
hint: its remote counterpart. Integrate the remote changes (e.g.
hint: 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.
```

Discuss what this means.

# Stéphane has to rebase his view of `master`

So I need to rebase my change from origin.
Doing so, I will incorporate the change Evan pushed, which will generate a conflict.

In VSCode: Pallette > Git rebase (Pull)

In Gitkraken: Pull (discuss the various options) -> rebase

# In the meantime Joel has submitted a PR
While we were doing all this, Joel [has created a PR](https://github.com/snicoll-scratches/hyf-coach-bios/pull/4) for his own bio
In the PR, [he's made a mistake on purpose with markdown](https://github.com/snicoll-scratches/hyf-coach-bios/pull/4/commits/f77275e070dfb6ee2d23816809fdc2190c388d49).

Stéphane spent some time explaining what a PR is, what reviews are and how this is concretely used in project.

# Stéphane reviews the PR
Stéphane reviews the PR and ask Joel to fix the broken markdown syntax.

Joel [pushes an extra commit on his existing branch](https://github.com/snicoll-scratches/hyf-coach-bios/pull/4/commits/16cde45bf63fa1069908b110ef84efc839aff331). This updates the PR automatically.

# Stéphane Polish the PR
There is also a conflict that must be reslved.
Github provides several options for that but resolving the conflict locally is the most powerful by far.

The conflict is fixed via the UI

# Wrapping Up
The 3 issues have been closed
