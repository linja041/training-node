# training-node
nothing important

# Project Structure Overview

```bash
├── codegen.yml        # GraphQL Code Generator configuration file
├── deploy.sh          # Deploy shell script
├── docker-compose.yml # Docker deploy file
├── Dockerfile         # Docker image build file
├── global.d.ts        # Global type definition file
├── next.config.js     # Next.js configuration file
├── next-env.d.ts      # Next.js configuration file
├── nginx              # Nginx configuration files
├── node_modules       # Node modules
├── package-dev.sh     # Package development version shell script
├── package.json
├── package-prod.sh    # Package production version shell script
├── pages              # Pages
├── public             # Public files
├── README.md
├── src                      # Source files
│   ├── assets              # Static files
│   ├── components          # All components
│   ├── containers          # Global contianers
│   ├── generated           # Generated files
│   ├── graphql             # GraphQL files
│   ├── models              # Global models
│   ├── react-app-env.d.ts
│   ├── theme.tsx           # Theme
│   ├── @types              # Custom type definition
│   └── utils               # Utility functions
└── tsconfig.json      # Typescript configuration file
```

# Style Guideline

## Global Common Components

Global common components must put in the `src/components/common`

## Page's Components

Page's components muse put in the `src/components`

Here is an example:

```bash
├── pages
│   └── dashboard  # Dashboard page
└── src
     └── components
          └── dashboard      # Dashboard page folder
               ├── component-a.tsx # Single subcomponent
               ├── component-b.tsx # Single subcomponent with folder
               │   ├── component-b-sub.tsx
               │   └── index.tsx
               └── index.tsx # Dashboard root page component
```

## Great Component Structure Layout

```bash
./src/components/button
├── index.tsx      # Root file
├── label.tsx      # Single subcomponent
└── rich-text      # Single subcomponent(Use folder if it has subcomponents)
    ├── audio.tsx   # Subcomponent's component
    ├── image.tsx   # Subcomponent's component
    └── index.tsx   # Subcomponent root file
```
