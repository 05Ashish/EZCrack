# Contributing

Thanks for your interest in contributing to EZCrack. We're happy to have you here.

Please take a moment to review this document before submitting your first pull request. We also strongly recommend that you check for [open issues](https://github.com/05Ashish/EZCrack/issues) and pull requests to see if someone else is working on something similar.

If you need any help, feel free to reach out to [@05Ashish](https://x.com/05Ashish).

## Structure

```
├── src
│  ├── app
│  │  ├── api
│  │  │  ├── auth
│  │  │  ├── contributors
│  │  │  ├── questions
│  │  │  ├── subjects
│  │  │  └── units
│  │  ├── branch
│  │  │  └── [branchId]
│  │  │     └── semester
│  │  │        └── [semId]
│  │  │           ├── page.tsx
│  │  │           └── subject
│  │  │              └── [subjectId]
│  │  │                 ├── page.tsx
│  │  │                 └── unit
│  │  │                    └── [unitId]
│  │  │                       └── page.tsx
│  │  ├── contributors
│  │  ├── notice
│  │  ├── globals.css
│  │  ├── layout.tsx
│  │  └── page.tsx
│  ├── components
│  │  ├── contributors
│  │  ├── home
│  │  ├── layout
│  │  ├── notes
│  │  ├── questions
│  │  ├── semester
│  │  ├── shared
│  │  ├── subjects
│  │  ├── topics
│  │  ├── ui
│  │  └── units
│  ├── constants
│  ├── contexts
│  ├── hooks
│  ├── lib
│  ├── models
│  ├── services
│  ├── styles
│  ├── types
│  └── utils
├── public
└── .github
```

## Development

### Fork this repo

You can fork this repo by clicking the fork button in the top right corner of this page.

### Clone on your local machine

```bash
git clone https://github.com/05Ashish/EZCrack.git
```

### Navigate to project directory

```bash
cd EZCrack
```

### Install dependencies

```bash
npm install
```

### Set up environment variables

Create a `.env` file in the root directory:

```env
MONGODB_URI=your_mongodb_connection_string
```

### Run development server

```bash
npm run dev
```

The application will be available at http://localhost:3000/

## Commit Convention

Before you create a Pull Request, please check whether your commits comply with
the commit conventions used in this repository.

### 1. Commit Message Format

When you create a commit we kindly ask you to follow the convention
`category(scope or module): message` in your commit message while using one of
the following categories:

- `feat / feature`: all changes that introduce completely new code or new features
- `fix`: changes that fix a bug (ideally you will additionally reference an issue if present)
- `refactor`: any code related change that is not a fix nor a feature
- `docs`: changing existing or creating new documentation
- `build`: all changes regarding the build of the software, changes to dependencies or the addition of new dependencies
- `chore`: all changes to the repository that do not fit into any of the above categories

**Example:**

```
feat(subjects): add weightage calculation for topics
```

### 2. Use Imperative Present Tense

Always write commit messages in imperative present tense.

✅ **Correct:**

```
Add login validation
Fix memory leak in cache
Update README
Remove unused imports
```

❌ **Incorrect:**

```
Added login validation
Fixes memory leak
Updating README
```

## Request for a new feature

If you have a request for a new component or feature, please open a discussion or an issue on GitHub. We'll be happy to help you out.

## Code Style

- Follow the existing code style
- Use TypeScript for type safety
- Write meaningful component and variable names
- Comment complex logic
- Keep components modular and reusable

## Questions?

Feel free to open an issue or reach out to [@05Ashish](https://x.com/05Ashish) on X (Twitter) if you have any questions or need clarification.

Thank you for contributing to EZCrack! 🎉
