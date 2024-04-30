
# Next.js App Router Organized Project Structure

This repository contains a Next.js project structured to leverage the Next.js App Router for organized and modular file management. The project is designed to accommodate large applications with numerous features and components, promoting clear separation of concerns and scalability.

## Project Structure Overview

The project uses a customized directory structure where routable components and APIs are clearly separated from private utility functions, hooks, components, and configurations. This ensures that only the necessary files are exposed as routes, while helper files and modules remain private and organized.

### Key Directories:

- `app/`: Main application logic separated into specific areas like pages and APIs.
- `_components/`: Global reusable UI components.
- `_hooks/`: Custom React hooks for shared logic across components.
- `_features/`: Distinct application features like user charts and timers.
- `_types/`: Global TypeScript type definitions.
- `_lib/`: Shared utility functions and libraries.
- `_constants/`: Application-wide constants.
- `_config/`: Configuration settings for the application.

### Full Directory Tree

```
src/
├── app/
│   ├── _components/
│   │   ├── Button.tsx                   # Reusable button component
│   │   └── Modal.tsx                    # Reusable modal component
│   ├── _hooks/
│   │   └── useAuth.ts                   # Authentication hook
│   ├── _features/
│   │   ├── user-chart/
│   │   │   ├── ChartComponent.tsx       # Chart component for user analytics
│   │   │   └── useChartData.ts          # Hook for chart data
│   │   └── timer/
│   │       ├── TimerComponent.tsx       # Timer component
│   │       └── useTimer.ts              # Timer hook
│   ├── _types/
│   │   └── globalTypes.ts               # Global TypeScript types
│   ├── _lib/
│   │   └── utils.ts                     # Utility library functions
│   ├── _constants/
│   │   └── appConstants.ts              # Application-wide constants
│   ├── _config/
│   │   └── appConfig.ts                 # Application configuration settings
│   ├── api/
│   │   ├── home/
│   │   │   └── getHomeData.ts           # API for home data
│   │   ├── blog/
│   │   │   └── getBlogPosts.ts          # API for blog posts
│   │   └── user/
│   │       └── getUserDetails.ts        # API for user details
│   ├── home/
│   │   ├── page.tsx                     # Home page component
│   │   ├── components/
│   │   │   └── HeroSection.tsx          # Specific component for home page
│   │   └── server-actions/
│   │       └── fetchData.ts             # Server-side action for data fetching
│   └── blog/
│       ├── page.tsx                     # Blog page component
│       ├── components/
│       │   └── BlogList.tsx             # Blog list component
│       ├── hooks/
│       │   └── useBlogData.ts           # Hook for fetching blog data
│       └── types/
│           └── blogTypes.ts             # TypeScript types for blog
└── styles/
    └── globals.css
```

## Usage

Clone this repository to begin a new Next.js project with a pre-organized structure. Navigate to your project directory and install the required dependencies:

```bash
npm install
```

Start the development server:

```bash
npm run dev
```

## Contributing

Contributions to improve the project structure or add new features are welcome. Please ensure to maintain the existing directory conventions and submit a pull request for review.

## License

This project is open-sourced under the MIT license. Feel free to use and modify it as per your requirements.
