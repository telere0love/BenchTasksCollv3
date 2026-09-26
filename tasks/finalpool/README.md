# Final Pool

This directory contains all tasks that have been verified to meet the requirements
specified in `tasks/examples/example-task`.

## Requirements for a task to be included in the final pool

A task is considered **implemented** and eligible for inclusion when it satisfies
all of the following requirements derived from `tasks/examples`:

1. `task_config.json` exists at the root of the task directory and contains:
   - a non-empty `needed_mcp_servers` field
   - a non-empty `needed_local_tools` field that includes `claim_done`
2. `docs/task.md` exists, is non-empty, and contains only English (no Chinese)
3. `docs/agent_system_prompt.md` exists, is non-empty, and contains only English
4. `docs/user_system_prompt.md` (optional) - if non-empty, must be all English
5. Other files/directories (e.g. `evaluation/`, `preprocess/`, `initial_workspace/`,
   `groundtruth_workspace/`) are optional; only their existence needs to be checked.

## Current Status

After auditing all developer branches in this repository, **no task currently
satisfies all of the requirements above**. Specifically, every task is missing
the required `task_config.json` file at the root of its directory.

Therefore, the final pool is currently empty. Tasks will be added to this
directory as they are completed and verified against the requirements.
