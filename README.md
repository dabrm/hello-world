# hello-world
Testing github

some random crapp here
and here

-- usefull commands

-- could not clone repo into LTQ machine - needed change proxy settings in Git
git config --global http.proxy http://proxy:8080/accelerated_pac_base.pac
-- where http://proxy:8080/accelerated_pac_base.pac is proxy package that LTQ uses


--To compare a local working directory against a remote branch, for example origin/master:

git fetch origin master
This tells git to fetch the branch named 'master' from the remote named 'origin'.  Git fetch will not affect the files in your working directory; it does not try to merge changes like git pull does.

git diff --summary FETCH_HEAD
When the remote branch is fetched, it can be referenced locally via FETCH_HEAD. The command above tells git to diff the working directory files against FETCHed branch's HEAD and report the results in summary format. Summary format gives an overview of the changes, usually a good way to start. If you want a bit more info, use --stat instead of --summary.

git diff FETCH_HEAD -- mydir/myfile.js
If you want to see changes to a specific file, for example myfile.js, skip the --summary option and reference the file you want (or tree).

--extra line added locally to test diff/fetch 
