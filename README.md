Antigravity Template
====================

This is a project template with customizations for Google's Antigravity.

It comes with three (very) opinionated playbooks that describe three phases of a project. These playbooks are implemented as workspace rules in Antigravity.

1. requirements-engineering-playbook.md (Phase 1)
2. solution-architecture-playbook.md (Phase 2)
3. software-development-playbook.md (Phase 3)

For each playbook, a corresponding workspace workflow is provided that activates the playbook when run.

- `/requirements` (Phase 1)
- `/architecture` (Phase 2)
- `/development` (Phase 3)


Usage
=====

1. Rename the template directory to your project name.
2. Go to "Customizations, Rules" in Antigravity, click on each playbook and set the "Activation Mode" to "Manual".
3. Review and adapt the playbooks to your needs. They are truly opinionated and you may disagree with some of the choices. But the format has proven to work well with various LLMs.
4. Start a new conversation in Antigravity and activate the playbook you want to use. Do not switch to another playbook within the same conversation. Always start a new conversation for each playbook and activate the playbook with the corresponding workflow (`/requirements`, `/architecture`, `/development`).
5. Note that Phases 2 and 3 expect files to be present that are created in the previous phases. In that sense, this template is intended for greenfield projects. For brownfield projects, you could try to reverse engineer the existing codebase and create a requirements document and architecture description by going through the Requirements Engineering and Solution Architecture playbooks before starting the Software Development playbook.
6. Delete this README.md file. A proper README.md for your project will be created by the Software Development playbook.