# gitpullrun

Usage: `gitpullrun REPO BRANCH COMMAND` will retrieve the current head of the given branch in the given repository and then run the command on it.

Features:
 * the tool will use --sparse to only download the needed stuff
 * the tool will cache the repo's branch head and fix any changes made to the cached repo directory that are within reason, then try to pull the current head
 * if you want to force a clone, set the environment variable `GPR_FORCE_CLONE=yes`
 * if you want to use a specific cache directory, set the environment variable `GPR_DIRECTORY=...` to point to it

