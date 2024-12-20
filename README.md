# git-breadcrumb

## Description 

Git Breadcrumbs to have automatic commits while not disturbing your main branch.

Those are most useful just before compilation or launching a test. As one often doesn't bother with commiting every compilation run. 

It creates a dedicated branch, starting from the current commit. And automatically commits everything there. It doesn't commit to the current branch since we don't want our usual workflow to be disrupted. And showing the difference between the last real commit to the current workspace is of paramount importance. Intermediate commits will stand in he way.

## Usage

Usage is very easy: 

Simply add the `git-breadcrumb` script in the PATH, and call `git breadcrumb`.

## Operation Mode

It will automatically update the branch `breadcrumb-$CURRENT_SHA1`, or create it if it doesn't exist yet.
