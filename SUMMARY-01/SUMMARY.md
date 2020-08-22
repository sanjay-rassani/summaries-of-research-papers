## Summary Of Paper – 01

### 1. Title, Authors, and Conference (where it was published):

**Title:** ***Need for Tweet: How Open Source Developers Talk About Their GitHub Work on Twitter.***

**Authors:** *(All the authors of this Paper are based in Carnegie Mellon University)*
***Hongbo Fang,***
***Daniel Klug,*** 
***Hemank Lamba,*** 
***James Herbsleb,*** and 
***Bogdan Vasilescu.***

**Conference:** MSR 2020

**Link to the Paper:** https://2020.msrconf.org/details/msr-2020-papers/27/Need-for-tweet-How-open-source-developers-use-Twitter-to-talk-about-their-GitHub-wor

### 2. Introduction:
In this Research Paper authors presented a computational approach to cross-link users over Twitter and GitHub, disclosing that more than 70,427 active users on both these open source platforms. By using this dataset, they analyzed on a case study of 786 tweets by open source developers about GitHub work, specifically tweets with links to GitHub repositories.
*[Also read the Related Work, precisely, in the Paper for a broader view.]*

### 3. Research Methodology:
By heuristic approach to cross-link GitHub and Twitter user accounts, based on computing GitHub user profile pages and personal blogs for direct URLs pointing to Twitter.
Identity merging approaches for user accounts in software repositories are based on heuristics and involve a precision-recall trade-off. 
Linking two accounts if they share the same email address tends to be a highly precise heuristic but with low recall (many people have multiple email addresses and they would not be linked this way). 
Matching people based on names is expected to have lower precision as common names are shared by many people, but higher recall (more accounts would get merged).
By using MySQL dump, they compiled a list of all GitHub user logins (excluding organizational and deleted accounts), then using the GitHub API to mine, for each user, their profile page blog URL field (which is not part of MySQL GHTorrent dump). If the target of the URL is a Twitter profile, then they assumed the linked Twitter account and the GitHub account belong to the same person and they recorded this account pair. If the URL points to a non-Twitter page, they crawled the content of that website for URLs pointing to Twitter; if the page only contains one such URL pointing to a Twitter profile, they assumed the linked Twitter account and the GitHub account belong to the same person and they recorded this pair; otherwise, they don’t record any link. This way they identified 72,668 GitHub-Twitter user account pairs.
*Final dataset consisting of 70,427 GitHub-Twitter user ID pairs: https://zenodo.org/record/3711630*

### 4. Result:
They didn’t performed a formal statistical analysis, their results seemed to suggest that GitHub project role and Twitter posting patterns are related. 
Conclusion from the Paper: Cross-linking data across online platforms where open source developers participate (in this paper GitHub and Twitter) is feasible and it can help provide deeper insights into how the activities of developers on one platform are moderated by the roles they play on the other. The social media activities of developers may also have direct impact on software development outcomes, including open-source project success. We provide a large dataset mapping 70,427 open-source developer GitHub and Twitter accounts, as basis for future (quantitative) empirical research in these directions.

