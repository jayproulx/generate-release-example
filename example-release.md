## What does a release look like?
===

	$ cat README.md 
	Welcome
	=======

	Current Version: 1.0.1

	$ cat package.json 
	{
	  "version": "1.0.1"
	}

	$ generate-release
	? Release Type patch
	? Are you sure you want to update the release from 1.0.1 to 1.0.2 Yes
	 ⫸  GIT: Pull from Origin                         Complete 
	 ⫸  GIT: Start Release                            Complete 
	 ⫸  Files: Write New Version                      Complete                 
	 ⫸  Commands: Pre Commit                          Complete 
	 ⫸  GIT: Commit Files                             Complete 
	 ⫸  Commands: Post Commit                         Complete 
	 ⫸  GIT: Finish Release                           Complete 
	 ⫸  GIT: Push to Origin                           Complete 
	 ⫸  Commands: Post Complete                       Complete 

	$ cat README.md 
	Welcome
	=======

	Current Version: 1.0.2

	$ cat package.json 
	{
	  "version": "1.0.2"
	}

## Looking at the Tree
===

![Image of Tree](/example-release.png)