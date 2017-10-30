# git workflow
#### 516030910199 ChenNuo

****


>## What is *git workflow*?  
   >* A useful tool for "Version Control Sustem".  
   >* The way that the product grows and be developed is similar to flow, thus been described as workflow.

****

>## How does *git workflow* works
    >### 1. *branches* and *merge*  
        >* A *branch* stores a perticular version for the project.  
        >*  When *merge* is done between two branches, one branch merges into the other(replaced by the former one).  
        >*  Different branches are created for different uses or versions.  
        >* When new pull down, new branches will be merged into appropriate branches and be deleted.  
    >### 2. regualtions for branches
        >* *master*  
            >   * Long time branch  
            >   * This branch stores the product which is released to users, and suppose to be steady.  
            >   * Only two kinds of braches that should grow from *master*:  
                >       * *develop*  
                >       * *hotfix ( fixbug )*  
        >* *develop*  
            >   * Long time branch  
            >   * This branch is stores the version which is under developing.  
            >   * Other braches are developed from this brach.   
        >* *hotfix ( fixbug )*  
            >   * Short time branch  
            >   * When bug(s) are reported from users ( means bug(s) appear in *master* ), *hotfix* is rose from *master*, and after bug(s) are fixed, *master* will merge this new version.
            >   * Will be deleted immediately when bug(s) are fixed.  
        >* *feature*
            >   * Short time branch
            >   * Used for developing new features  
            >   * merge *develop* and *master* when new version passes all tests.  
            >   * Will be deleted immediately after merges.  
        >* *release*  
            >   * Short time branch  
            >   * Used for release( develping at the same time ).  
            >   * Will be deleted immediately after  

****

>## Why should we choose *git workflow*?  
    >### 1. compare with *SVN*