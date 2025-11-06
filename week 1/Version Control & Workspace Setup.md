## Version Control

### 1. Git

**Git** is a **fast, scalable, distributed revision control system** with an unusually rich command set that provides both high-level operations and full access to internals.

* It is the **core technology** that most modern version control platforms are built upon.
* Its **distributed** nature means every developer has a full copy of the entire repository's history, allowing for offline work and resilient data.

---

### 2. GitLab

**GitLab** is a **web-based DevOps platform** that provides a single application for the entire software development lifecycle.

* It **integrates** version control (using Git), CI/CD pipelines, issue tracking, and project management.
* It's known as a comprehensive, **"all-in-one" solution**.
* It offers the ability to be **self-hosted** for greater control, distinguishing it from services like GitHub.

---

### 3. Bitbucket

**Bitbucket** is a web-based, **Git-based source code hosting and collaboration tool** for software development teams, owned by Atlassian.

* It allows teams to manage their code, track changes, and collaborate using features like branching and merging.
* It offers built-in tools for **CI/CD**.
* Its key strength is its **deep integration with other Atlassian products** like Jira and Trello.
* It is available as both a **cloud-based service** and a **self-hosted "Data Center"** solution.

---


# Project setup

---

## 1. Working with Feature Branches

A **feature branch** is a separate line of development in a version control system (like **Git**) where a developer works on a new feature, bug fix, or enhancement without affecting the main codebase.

* **Purpose:** To provide a safe, dedicated space for development, allowing multiple developers to work in parallel without interfering with each other or destabilizing the main branch.
* **Isolation:** The work is kept isolated from the main (e.g., "master" or "main") branch until it is complete, reviewed, and tested.
* **Workflow:** Once the work is complete and tested, the feature branch is merged back into the main branch, integrating the changes into the official release codebase.

---

## 2. Staging/User Acceptance Testing (UAT) Branch

A **staging/UAT branch** serves as a **near-perfect replica of the production environment** for final testing before a release. It ensures the software is ready for deployment and meets business needs.

The branch serves two distinct purposes: **Staging** and **UAT**.

| Phase | Purpose | Who Tests | Focus |
| :--- | :--- | :--- | :--- |
| **Staging** | To test the final code in a production-like environment to catch any remaining technical bugs, configuration issues, or deployment problems. | Developers and Quality Assurance (QA) engineers. | **Technical validation**, performance, and compatibility testing. |
| **UAT (User Acceptance Testing)** | To ensure the software meets the business requirements and provides a good user experience from the end-user's perspective. | End-users, business analysts, or product owners. | **User-centric validation**, usability, and business workflow testing. It is the final sign-off phase. |

---

## 3. Production Branch

The **production branch** (often named `main` or `master`) represents the version of the software that is **live and visible to end-users**.

* **Role:** It holds the **most current, stable, and approved code** that is ready for release or currently deployed.
* **Status:** It is the "source of truth" for the stable product.
* **Workflow:** Development work happens in feature branches, which are then integrated (via staging/UAT) into the production branch once they are proven stable and correct.

---
