usethis::create_github_token()

* Call `gitcreds::gitcreds_set()` to register this token in the local Git credential store
It is also a great idea to store this token in any password-management software that you use
??? Opening URL 'https://github.com/settings/tokens/new?scopes=repo,user,gist,workflow&description=R:GITHUB_PAT'

gitcreds::gitcreds_set()


-> Your current credentials for 'https://github.com':

protocol: https
host    : github.com
path    :
username: PersonalAccessToken
password: <-- hidden -->

-> What would you like to do?

1: Keep these credentials
2: Replace these credentials
3: See the password / token


Selection: 2

-> Removing current credentials...

? Enter new password or token: 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
-> Adding new credentials...
-> Removing credetials from cache...
-> Done.

usethis::create_from_github("aosmith16-testing/pull-practice")
i Defaulting to 'https' Git protocol
√ Setting `fork = TRUE`
√ Creating 'C:/Users/ariel/Desktop/pull-practice/'
√ Forking 'aosmith16-testing/pull-practice'
√ Cloning repo from 'https://github.com/aosmith16/pull-practice.git' into 'C:/Users/ariel/Desktop/pull-practice'
√ Setting active project to 'C:/Users/ariel/Desktop/pull-practice'
i Default branch is 'master'
√ Adding 'upstream' remote: 'https://github.com/aosmith16-testing/pull-practice.git'
√ Pulling changes from 'upstream/master' (default branch of source repo)
√ Setting remote tracking branch for local 'master' branch to 'upstream/master'
√ Writing 'pull-practice.Rproj'
√ Adding '.Rproj.user' to '.gitignore'
√ Opening 'C:/Users/ariel/Desktop/pull-practice/' in new RStudio session
√ Setting active project to '<no active project>'

# Then opens new RStudio session
usethis::pr_init(branch = "acmpractice2")

√ Setting active project to 'C:/Users/ariel/Desktop/pull-practice'
√ Pulling changes from 'upstream/master'
√ Creating and switching to local branch 'acmpractice'
* Use `pr_push()` to create PR.

# Make changes then commit
usethis::pr_push()

√ Pushing local 'acmpractice' branch to 'origin' remote
* Create PR at link given below
√ Opening URL 'https://github.com/aosmith16/pull-practice/compare/acmpractice'

# After merging
usethis::pr_finish()

√ Switching back to default branch ('master')
√ Pulling changes from 'upstream/master'
√ Deleting local 'acmpractice' branch
√ PR 'aosmith16-testing/pull-practice/#9' has been merged, deleting remote branch 'origin/acmpractice'

