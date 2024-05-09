# github-actions-repo
Test repository for working with Linux self-hosted GitHub runners.

## Set up the runner
Download the latest runner [here](https://github.com/actions/runner/releases).

Create the directories for the runner and unpack them (using a version below):
```bash
mkdir \actions-runner ; cd \actions-runner
curl -O -L https://github.com/actions/runner/releases/download/v2.316.1/actions-runner-linux-x64-2.316.1.tar.gz
tar xzf ./actions-runner-linux-x64-2.316.1.tar.gz
```

Ensure you assign a runner token from your GitHub repo via your repositories *Settings->Actions->Runners->New self-hosted runner*.

Configure the runner to activate it:
```
./run.sh
```
