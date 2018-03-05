# imperative-when
Use when statement in imperative pipeline inkl. Blue Ocean shows skipped stages

## Usage

### Include in Jenkins

Define a global pipeline library that uses this repo. Enable "Load implicitly" if you like.

### Example Pipeline code

    stage('Zero') {
        when(BRANCH_NAME != 'master') {
            echo 'Performing steps of stage Zero'
        }
    }
