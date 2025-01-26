# Laravel Dev Kit

Laravel Dev Kit is a starter kit for Laravel applications, designed to save time and set up your projects with a standardized environment. It includes pre-configured tools for code linting, formatting, and CI/CD workflows, ensuring code quality and consistency.

---

## Features

- **CI/CD Workflows**: Pre-configured GitHub Actions workflows for:

    - PHP linting
    - Fixing common coding issues
    - Prettier integration
    - Automated testing with Laravel

- **Husky Pre-Commit Hooks**: Automatically run linting and formatting tasks before committing changes.

- **Linting and Formatting**:

    - `LaraStan` for static analysis
    - `Pint` for PHP code formatting
    - Prettier for JavaScript, CSS, and other frontend assets
    - `postcss` for processing CSS

- **Custom Configuration Files**:
    - `.prettierrc` and `.prettierignore` for Prettier
    - `lint-staged.config.js` for staged file linting
    - `phpstan.neon.dist` for PHPStan configuration
    - `pint.json` for Pint settings
    - `.git-blame-ignore-revs` for ignoring certain commits in git blame output

---

## File Structure

```plaintext
/
|-- .gitHub
|   |-- workflows
|   |   |-- duster-fix-blame.yml
|   |   |-- laravel.yml
|   |   |-- lint.yml
|   |   |-- prettier-write.yml
|
|-- .husky
|   |-- _
|   |   |-- .gitignore
|   |   |-- husky.sh
|   |-- pre-commit
|
|-- .prettierrc
|-- .git-blame-ignore-revs
|-- .prettierignore
|-- lint-staged.config.js
|-- phpstan.neon.dist
|-- pint.json
|-- postcss.config.js
```

---

## Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) (for frontend tooling)
- [Composer](https://getcomposer.org/) (for PHP dependencies)
- A fresh Laravel application

### Installation

1. Clone the repository:

    ```bash
    git clone https://github.com/shaz3e/laravel-dev-kit.git my-new-app
    cd my-new-app
    ```

2. Install PHP dependencies:

    ```bash
    composer install
    ```

3. Install Node.js dependencies:

    ```bash
    npm install
    ```

4. Configure Husky hooks:

5. Customize `.env` for your Laravel application.

### Usage

1. Run the local development server:

    ```bash
    php artisan serve
    ```

2. Watch and build frontend assets:

    ```bash
    npm run dev
    ```

3. Commit code with pre-commit checks automatically applied.

---

## Workflows

### GitHub Actions

The `.github/workflows` folder includes:

- **duster-fix-blame.yml**: Automatically fix coding standards and blame-ignore files.
- **laravel.yml**: Run tests and ensure application stability.
- **lint.yml**: Run PHP, CSS, and JS lint checks.
- **prettier-write.yml**: Enforce Prettier standards across supported files.

### Husky Hooks

Automatically lint and format files before committing changes. Customize the hook behavior in `.husky/pre-commit`.

---

## Contributing

Contributions are welcome! Feel free to submit a pull request or open an issue for discussion.

---

## License

This repository is open-source and available under the [MIT License](LICENSE).

---

## Acknowledgments

Laravel Dev Kit simplifies the setup process for Laravel applications, integrating essential developer tools to streamline workflows and maintain code quality.

## Credit

This project utilizes and integrates various tools and resources to provide an optimized development experience. Special thanks to:

- aravel: For providing a robust PHP framework.
- LaraStan: For powerful static analysis tailored to Laravel applications.
- PHPStan: A static analysis tool that ensures code quality.
- Pint: Laravel's official code formatter for PHP.
- Prettier: An opinionated code formatter for JavaScript, CSS, and more.
- Husky: For Git hooks management to automate checks and ensure quality.
- Lint-Staged: For running linters against staged Git files.
- PostCSS: For CSS transformations and optimizations.
- GitHub Actions: For seamless CI/CD workflows.

We acknowledge these open-source tools, frameworks, and the global development community for their contributions.

If you'd like to be recognized as a contributor to this repository, feel free to submit a pull request or raise an issue with solution.
