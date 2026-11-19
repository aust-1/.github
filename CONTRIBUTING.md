# Contributing

Thank you for your interest in contributing to this repository! To ensure a smooth and collaborative process, please follow these guidelines.

## Before You Start

Before making any changes, please discuss the proposed change with the repository owners. You can do this via an issue, email, or any other communication method.

## Code of Conduct

Please adhere to our [Code of Conduct](./CODE_OF_CONDUCT.md) in all your interactions with the project.

## Internationalization (I18N)

Contributions (documentation, issues, pull requests and commit messages) should be written in the language of the repository, which is the language of its `README.md`: French for most repositories, English for the others.

Translations can be provided in addition to the main version. It is recommended to use the [ISO 639-1](https://en.wikipedia.org/wiki/List_of_ISO_639-1_codes) standard for language codes.

## Code Style Guidelines

For all contributions, please follow these code style guidelines:

- Maintain consistent naming conventions across the entire codebase.
- Keep functions concise and focused on a single responsibility.
- Include unit tests for every new feature or bug fix to ensure reliability.

## Documentation

Documentation is mandatory for all contributions, including code, issues, and pull requests. The documentation should be:

- Clear and concise
- Written in Markdown format
- Included in the `README.md` file at the root of the project
- Additional documentation can be added to the `docs` folder

## Deployment

Projects meant to run as a long-lived service on a server (website, API, bot) should provide a Docker deployment option: a `Dockerfile` if necessary and a Compose file, named either `compose.yml` or `docker-compose.yml`. Command-line tools, libraries, notebooks and mobile apps do not need one. The deployment process should be:

- As simple as possible
- Documented in the `README.md` file

## Testing

All contributions should include tests to ensure the stability and reliability of the project. Please follow these guidelines for testing:

- Write unit tests for new functionality and bug fixes.
- Use a testing framework appropriate for the project's language and environment.
- Ensure that all tests pass before submitting a pull request.
- Include instructions on how to run the tests in the README.md file.

## Commit Messages

All commit messages should follow the [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/) format. This format ensures that the commit messages are easy to read and follow a consistent structure.

The use of emojis in commit messages is encouraged to make the messages more engaging and easier to understand.

## Git strategy

Most repositories use a simple branching model:

- The default branch (`main`, or `master` in a few older repositories) should always be stable and deployable.
- Every change is made on a short-lived branch created from the default branch, then merged through a pull request.

Branch names follow the `<type>_<short_description>` pattern, with underscores, for example `fix_oauth_code_logs` or `docs_security_policy`. The type is one of:

- `feature_*`: new functionality.
- `fix_*`: bug fixes.
- `docs_*`: documentation only.
- `ci_*`: continuous integration and workflows.
- `chore_*`: maintenance (dependencies, tooling, cleanup).

Repositories that have a `dev` branch follow the [GitFlow](https://www.atlassian.com/git/tutorials/comparing-workflows/gitflow-workflow) branching model instead: branches are created from `dev` and merged back into it, and `dev` is merged into the default branch for each release. In these repositories, `hotfix_*` branches for critical fixes are created from the default branch and merged into both the default branch and `dev`.

Check the repository's `README.md` for any specific rule.

---

By following these guidelines, you help ensure that the project remains well-organized, accessible, and collaborative. Thank you for your contributions!
