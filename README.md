Antigravity Template
====================

This is a template for a new project using Antigravity.

It comes with three (very) opinionated playbooks that describe three phases of a project. These playbooks are implemented as workspace rules in Antigravity.

1. requirements-engineering-playbook.md (phase 1)
2. solution-architecture-playbook.md (phase 2)
3. software-development-playbook.md (phase 3)

For each playbook, a corresponding Antigravity workflow is provided that activates the playbook when run.

- `/requirements` (phase 1)
- `/architecture` (phase 2)
- `/development` (phase 3)


Usage
=====

1. Rename the template directory to your project name.
2. Review and adapt the playbooks to your needs. They are truly opinionated and you may disagree with some of the choices. But the format has proven to work well with various LLMs.
3. Start a new conversation in Antigravity and activate the playbook you want to use. Do not switch to another playbook within the same conversation. Always start a new conversation for each playbook and activate the playbook with the corresponding Antigravity workflow (`/requirements`, `/architecture`, `/development`).
4. Note that phase 2 and 3 expect files to be present that are created in the previous phases. In that sense, this template is intended for greenfield projects. For brownfield projects, you could try to reverse engineer the existing codebase and create a requirements document and architecture description by going through the Requirements Engineering and Solution Architecture playbooks.