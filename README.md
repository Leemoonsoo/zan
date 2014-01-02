# Zeppelin Archive Network

Zeppelin Archive Network is central library repository for [Zeppelin](http://zeppelin-project.org). 

### Publishing your own library

1. Fork and clone https://github.com/NFLabs/zan
2. Create directory with your library name
3. Create 'meta' file inside of the directory
4. Optionally create 'README.md' in the directory
5. Commit, push your directory and make pull request.

#### 'meta' file spcification

Meta file is json formatted text file


      {
            "repository" : "[REPOSITORY URL]",
            "branch"     : "[BRANCH NAME]",
            "commit"     : "[COMMIT HASH]"
      }


