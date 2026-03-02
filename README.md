<<<<<<< test/TP2-T1299
# Advance Git Asessment
* Create a branch develop from the main
    ```
    git checkout -b develope 
    ```
* Add a commit message hook to the repo.
    - Create the hook file
    - Make it executable
    - Write validation logic
        ``` 
        #!/bin/sh

        commit_msg=$(cat "$1")

        if ! echo "$commit_msg" | grep -E "^(feat|fix|docs|style|refactor|test|chore):" > /dev/null
        then
        echo "Invalid commit message format."
        echo "Use: feat:, fix:, docs:, style:, refactor:, test:, chore:"
        exit 1
        fi
        ```
    
* Perform multiple commits in the branch
    - Modified the READMD.md file
        ``` 
            git commit -m "test: T12-T1299-02 modified the README.md
        ```
    - Added the new text file
        ```
            git commit -m "test: TP2-T1299-04 - add new text file
        ```
    - Modified the text file
        ```
            git commit -m "test: TP2-T1299-05 - modify the text document
        ```
    - MOdified the README.md file
        ```
            git commit -m "test: TP2-T1299-05 - modify the README.md
        ```
=======
# Advance git assessment
>>>>>>> develop
