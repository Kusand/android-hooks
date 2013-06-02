android-hooks
=============

A potentially useful pre-commit hook for Android developers using git.


pre-commit.lintcheck
--------------------

The lintcheck pre-commit hook runs __lint --exitcode .__ before allowing a commit to occur. If lint returns a non-zero exit code, it will fail the commit. Users can customize their hook using git config values for _hooks.lintTargetDirectory_ to change the directory to check and _hooks.lintArgs_ to add lint arguments they prefer to use, such as _-Werror_.