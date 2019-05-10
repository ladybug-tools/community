# Community

Ladybug Tools community content


## Links of Interest

### Semantic Versioning

* https://en.wikipedia.org/wiki/Software_versioning

	Software upgrade versioning is the process of assigning either unique version names or unique version numbers to unique states of computer software. Within a given version number category (major, minor), these numbers are generally assigned in increasing order and correspond to new developments in the software. At a fine-grained level, revision control is often used for keeping track of incrementally different versions of information, whether or not this information is computer software.

* https://semver.org/

	Given a version number MAJOR.MINOR.PATCH, increment the:

	MAJOR version when you make incompatible API changes,
	MINOR version when you add functionality in a backwards-compatible manner, and
	PATCH version when you make backwards-compatible bug fixes.
	Additional labels for pre-release and build metadata are available as extensions to the MAJOR.MINOR.PATCH format.

* A brief guide to Semantic Versioning / https://medium.com/@jameshamann/a-brief-guide-to-semantic-versioning-c6055d87c90e

	Before publishing your first, useable version, you might find yourself incrementing the middle and the last digit to keep track of Alpha/Beta releases. Only once you’re ready for a proper, first release, should you start versioning from 1.0.0.

* About semantic versioning /https://docs.npmjs.com/about-semantic-versioning

	To keep the JavaScript ecosystem healthy, reliable, and secure, every time you make significant updates to an npm package you own, we recommend publishing a new version of the package with an updated version number in the package.json file that follows the semantic versioning spec. Following the semantic versioning spec helps other developers who depend on your code understand the extent of changes in a given version, and adjust their own code if necessary.

* semantic-pedantic.md / https://gist.github.com/jashkenas/cbd2b088e20279ae2c8e

	If you pretend like SemVer is going to save you from ever having to deal with a breaking change — you're going to be disappointed. It's better to keep version numbers that reflect the real state and progress of a project, use descriptive changelogs to mark and annotate changes in behavior as they occur, avoid creating breaking changes in the first place whenever possible, and responsibly update your dependencies instead of blindly doing so.

	* Many interesting comments to a short gist
	* Asks for: "Romantic Versioning"

* Semantic Versioning 101 / https://hackernoon.com/semantic-versioning-101-d2623083714b

	Semantic versioning is for your consumers. It’s not for your release schedule or your marketing plan.


### Commit Messages

* https://en.wikipedia.org/wiki/Commit_(version_control)

	In version control systems, a commit adds the latest changes to [part of] the source code to the repository, making these changes part of the head revision of the repository. Unlike commits in data management, commits in version control systems are kept in the repository indefinitely. Thus, when other users do an update or a checkout from the repository, they will receive the latest committed version, unless they specify they wish to retrieve a previous version of the source code in the repository. Version control systems allow rolling back to previous versions easily. In this context, a commit within a version control system is protected as it is easily rolled back, even after the commit has been applied.

* Victor Parmar/ The case for single character git commit message prefixes / https://smalldata.tech/blog/2018/10/04/the-case-for-single-character-git-commit-message-prefixes

	* B, indicates a bugfix.
	* F, indicates a feature or a change - this will most likely be the majority of the commits.
	* a, code formatting change.
	* c, comments and or documentation.
	* D, dependency updates.
	* R, code refactoring, note that this is different from r below.
	* r, proven code refactoring - this is the original meaning of the mathematical term refactoring, where it can be mathematically proven that the code change does not change any functionality.
	* T, test cases and/or test improvements
	* !, unknown - i.e. for when you really need to make that commit because there's a horde of zombies waiting outside.

* Conventional Commits 1.0.0-beta.4

	The Conventional Commits specification is a lightweight convention on top of commit messages. It provides an easy set of rules for creating an explicit commit history; which makes it easier to write automated tools on top of. This convention dovetails with SemVer, by describing the features, fixes, and breaking changes made in commit messages.

* https://github.com/RomuloOliveira/commit-messages-guide

	A guide to understanding the importance of commit messages and how to write them well.

	Why are commit messages important?
	To speed up and streamline code reviews
	To help in the understanding of a change
	To explain "the whys" that cannot be described only with code
	To help future maintainers figure out why and how changes were made, making troubleshooting and debugging easier
	To maximize those outcomes, we can use some good practices and standards described in the next section.

* Useful Tips for writing better Git commit messages / https://code.likeagirl.io/useful-tips-for-writing-better-git-commit-messages-808770609503

	* Some Rules to keep in mind when writing commit messages
	* Separate subject from body with a blank line
	* Limit the subject line to 50 characters
	* Capitalize the subject line
	* Do not end the subject line with a period
	* Use the imperative mood in the subject line
	* Wrap the body at 72 characters
	* Use the body to explain what and why vs. how

* commit-message-guidelines.md / https://gist.github.com/robertpainsi/b632364184e70900af4ab688decf6f53


* https://wiki.openstack.org/wiki/GitCommitMessages#Information_in_commit_messages

	The cardinal rule for creating good commits is to ensure there is only one "logical change" per commit. There are many reasons why this is an important rule:

	* The smaller the amount of code being changed, the quicker & easier it is to review & identify potential flaws.
	* If a change is found to be flawed later, it may be necessary to revert the broken commit. This is much easier to do if there are not other unrelated code changes entangled with the original commit.
	* When troubleshooting problems using Git's bisect capability, small well defined changes will aid in isolating exactly where the code problem was introduced.
	* When browsing history using Git annotate/blame, small well defined changes also aid in isolating exactly where & why a piece of code came from.
