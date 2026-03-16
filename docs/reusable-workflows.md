# Reusable Workflows

- Shall have _on.workflow\_call_ event
- Does not define _environment_ (i.e., you can **not** access _env_ to set inputs from the caller)
- If it is just a workflow (i.e., not an Action), you shall define types for the inputs
- If the reusable workflow is defined in the same project, you can access it without specifying a Git Ref or an action version (i.e., the path to the YAML file suffices)
- The reusable workflow shall be defined in the `.github/workflow/` folder (the workflow folder does **not** support subfolders to discover workflows
